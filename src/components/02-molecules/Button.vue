<template>
    <input class="common u-text-body_medium" type="submit" :value="text" v-if="submit">
    <a class="common u-text-body_medium" :href="link" v-else>{{text}}</a>
</template>

<script>
export default {
  name: 'Button',
  props: {
    text: String,
    link: String,
    submit: Boolean
  }
}
</script>

<style scoped lang="scss">
.common {
    padding: 14px 48px;
    border-radius: 4px;
    border: none;
    color: var(--light-neutral-n-1);
    cursor: pointer;
    font-family: "HelveticaNeue";
    font-weight: 500;
}
a {
    background: var(--light-accent-accent-base);
}
input {
    background: var(--light-primary-primary-base);
}
</style>