<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <HelloWorld msg="Welcome to Your Vue.js App"/>
  </div>
</template>

<script>
import HelloWorld from './components/05-pages/HelloWorld.vue'
import "./scss/style.scss";

export default {
  name: 'App',
  components: {
    HelloWorld
  }
}
</script>