<template>
  <div>
    <button class="button-default">
      <slot />
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

  background: radial-gradient(circle at 100% 100%, #ffffff 0, #ffffff 6px, transparent 6px) 0% 0%/8px 8px no-repeat,
            radial-gradient(circle at 0 100%, #ffffff 0, #ffffff 6px, transparent 6px) 100% 0%/8px 8px no-repeat,
            radial-gradient(circle at 100% 0, #ffffff 0, #ffffff 6px, transparent 6px) 0% 100%/8px 8px no-repeat,
            radial-gradient(circle at 0 0, #ffffff 0, #ffffff 6px, transparent 6px) 100% 100%/8px 8px no-repeat,
            linear-gradient(#ffffff, #ffffff) 50% 50%/calc(100% - 4px) calc(100% - 16px) no-repeat,
            linear-gradient(#ffffff, #ffffff) 50% 50%/calc(100% - 16px) calc(100% - 4px) no-repeat,
            linear-gradient(90deg, #961ef4 0%, #e35858 100%);
  border-radius: 8px;
  padding: 6px;
  box-sizing: border-box;
  border: none;
}
</style>