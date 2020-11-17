<template>
  <div>
    <TextComponent type="h1" msg="Profile Page" attribute="u-text-title" />
    <FormInput title="Login" type="email" placeholder="Jane Doe@gmail.com" other="null"/>
    <Button text="Save" />
    <Button text="Delete" submit />
    <Link class="u-text-menu_items" link="#" text="Profile"/>
    <Avatar class="u-text-menu_items u-avatar-little" placeholder="J"/>
    <Text text="Watch out, this function causes the complete and irreversible deletion of your nickname. It will no longer be usable and you will lose all associated data. Make sure this is what you want to do." />
  </div>
</template>

<script>
import FormInput from '../02-molecules/FormInput.vue'
import TextComponent from '../01-atoms/TextComponent.vue'
import Button from '../02-molecules/Button.vue'
import Text from '../01-atoms/Text.vue'
import Link from '../01-atoms/Link.vue'
import Avatar from '../01-atoms/Avatar.vue'
export default {
  name: 'AccountPage',
  components: {
    FormInput,
    TextComponent,
    Button,
    Text,
    Link,
    Avatar
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
</style>
