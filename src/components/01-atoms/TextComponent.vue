<template>
  <div>
    <h1 v-if="type === 'h1'" :class="attribute" >{{ msg }}</h1>
    <h2 v-if="type === 'h2'" :class="attribute" >{{ msg }}</h2>
    <h3 v-if="type === 'h3'" :class="attribute" >{{ msg }}</h3>
    <h4 v-if="type === 'h4'" :class="attribute" >{{ msg }}</h4>
    <h5 v-if="type === 'h5'" :class="attribute" >{{ msg }}</h5>
    <h6 v-if="type === 'h6'" :class="attribute" >{{ msg }}</h6>
    <p v-if="type === 'p'" :class="attribute" >{{ msg }}</p>
    <span v-if="type === 'span'" :class="attribute" >{{ msg }}</span>
  </div>
</template>

<script>
export default {
  name: 'TextComponent',
  props: {
    msg: String,
    type: String,
    attribute: String
  }
}
</script>