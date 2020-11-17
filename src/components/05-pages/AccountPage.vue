<template>
  <div>
    <TextComponent type="h1" msg="Profile Page" attribute="u-text-title" />
    <FormInput title="Login" type="email" placeholder="Jane Doe@gmail.com" other="null"/>
  </div>
</template>

<script>
import FormInput from '../02-molecules/FormInput.vue'
import TextComponent from '../01-atoms/TextComponent.vue'
export default {
  name: 'AccountPage',
  components: {
    FormInput,
    TextComponent
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
