<template>
    <div>
        <Avatar v-if="avatar" class="u-text-menu_items u-avatar-little" :placeholder="avatarPlaceholder"/>
        <Link class="u-text-menu_items" :link="link" :text="linkText"/>
    </div>
</template>

<script>
import Avatar from '../01-atoms/Avatar.vue'
import Link from '../01-atoms/Link.vue'
export default {
  name: 'SideBarItem',
  components: {
      Avatar,
      Link
  },
  props: {
    linkText: String,
    link: String,
    avatar: Boolean,
    avatarPlaceholder: String,
  }
}
</script>

<style scoped lang="scss">
div {
    display: flex;
    flex-direction: row;
    align-items: center;
    div+a {
        margin-left: 15px;
    }
}
</style>