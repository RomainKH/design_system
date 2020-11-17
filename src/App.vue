<template>
  <div id="app">
    <AccountPage/>
  </div>
</template>

<script>
import "./scss/style.scss";
import AccountPage from './components/05-pages/AccountPage.vue'

const html = document.querySelector('html')
html.dataset.theme = "light"
export default {
  name: 'App',
  components: {
    AccountPage
  }
}
</script>