<template>
    <div>
        <img v-if="image" :src="src" :alt="alt">
        <p v-else>{{ placeholder }}</p>
    </div>
</template>

<script>
export default {
  name: 'Link',
  props: {
    image: Boolean,
    src: String,
    alt: String,
    placeholder: String

  }
}
</script>

<style scoped lang="scss">
div {
    border-radius: 50%;
    background: var(--light-accent-accent-base);
    display: flex;
    align-items: center;
    justify-content: center;
}
p {
    color: var(--light-neutral-white);
}
</style>