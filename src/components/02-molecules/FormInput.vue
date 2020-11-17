<template>
  <div>
    <div v-if="other === 'null'" class="form_container">
      <label class="u-text-label label" :for="type" >{{ title }}</label>
      <input  class="form_input input" :type="type" :id="type" :name="type" required
      minlength="8" maxlength="20" size="20" :placeholder="placeholder">
    </div>
    <div v-if="other !== 'null'" class="form_container">
      <label class="u-text-label" :for="other" >{{ title }}</label>
      <textarea v-if="other === 'textarea'" :id="other" name="story" rows="5" cols="33">
        It was a dark and stormy night...
      </textarea>
      <!-- ADD ROMAIN MAILLOT !-->
    </div>
  </div>
</template>

<script>
export default {
  name: 'FormInput',
  props: {
    title: String,
    type: String,
    placeholder: String,
    other: String || null
  }
}
</script>

<style lang="scss" scoped>
  .form_container {
    display: flex;
    flex-direction: column;
  }
  .label {
    margin-bottom: 10px;
  }
  .input {
    padding: 12px 20px;
  }
</style>