<template>
  <div>
    <textarea
      class="teste"
      :placeholder="placeholder"
      :value="value"
      @input="$emit('input', $event.target.value)"
    />
  </div>
</template>
<script>
  export default{
    name: 'BaseTextarea',
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
.teste {
  width: 230px;
  height: 315px;
  resize: none;
  margin: 10px 5px;
}
</style>