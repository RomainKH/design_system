<template>
    <h1 v-if="ish1">{{ msg }}</h1>
    <h2 v-else>{{ msg }}</h2>
</template>

<script>
export default {
  name: 'Title',
  props: {
    msg: String,
    ish1: Boolean
  }
}
</script>