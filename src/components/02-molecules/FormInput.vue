<template>
  <div class="form_input">
    <label class="u-text-label" for="name" >{{ title }}</label>
    <input :type="whatType" id="name" name="name" required
    minlength="8" maxlength="20" size="20" pattern=".+@gmail.com" :placeholder="placeholder">
  </div>
</template>

<script>
export default {
  name: 'FormInput',
  props: {
    title: String,
    whatType: String,
    placeholder: String
  }
}
</script>

<style lang="scss" scoped>
  .form_input {
    display: flex;
    flex-direction: column;
    width: 300px;
  }
</style>