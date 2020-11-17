<template>
  <h1 class="u-text-title title-style" v-if="ish1">{{ msg }}</h1>
  <h2 class="u-text-sidebar_title title-style" v-else>{{ msg }}</h2>
</template>

<script>
import "../../scss/style.scss";
export default {
  name: 'Title',
  props: {
    msg: String,
    ish1: Boolean
  }
}
</script>
