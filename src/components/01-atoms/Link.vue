<template>
    <a :href="link">{{ text }}</a>
</template>

<script>
export default {
  name: 'Link',
  props: {
    link: String,
    text: String
  }
}
</script>

<style scoped lang="scss">
a {
    text-decoration: none;
    width: 100%;
}
</style>