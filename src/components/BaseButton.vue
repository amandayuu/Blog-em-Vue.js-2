<template>
  <div>
    <button class="button-default">
      <slot></slot>
    </button>
  </div>
</template>
<script>
export default {
  name:"BaseButton",  
}
</script>
<style lang="scss">
.button-default {
  margin: 10px 5px;
  width: 230px;
  height: 40px;
}
</style>