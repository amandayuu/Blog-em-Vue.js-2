<template>
  <div>
    <input 
      class="input-component" 
      :placeholder="placeholder"
      :value="value"
      @input="$emit('input', $event.target.value)"
    >
  </div>
</template>
<script>
export default {
  name: 'BaseInput',
  props: {
    placeholder: {
      type: String,
      required: true
    },
    value: {
      type: String,
      default: ''
    }
  }
}
</script>
<style lang="scss">
.input-component {
  height: 40px;
  width: 230px;
  margin: 10px 5px;
  border: 1px solid #939393;
  border-radius: 5px;
}
</style>