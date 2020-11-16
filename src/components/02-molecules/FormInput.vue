<template>
    <div>
      <label for="name" >{{ title }}</label>
      <input :type="whatType" id="name" name="name" required
      minlength="4" maxlength="8" size="10">
    </div>
</template>

<script>
export default {
  name: 'FormInput',
  props: {
    title: String,
    whatType: String
  }
}
</script>