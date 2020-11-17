<template>
  <div>
    <Title :ish1="true" msg="Profile Page" />
    <FormInput title="Login" whatType="email" placeholder="Jane Doe@gmail.com"/>
  </div>
</template>

<script>
import FormInput from '../02-molecules/FormInput.vue'
import Title from '../01-atoms/Title.vue'
export default {
  name: 'AccountPage',
  components: {
    FormInput,
    Title
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
