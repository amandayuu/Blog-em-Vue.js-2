<template>
  <div>
    <div class="item form">

      <div class="header">
        <span class="title">
          Form
        </span>
      </div>

      <BaseInput />
      <BaseInput />
      <textarea class="post-textarea" />
      <BaseButton />
    </div>
  </div>
</template>
<script>
  import BaseInput from './BaseInput.vue';
  import BaseButton from './BaseButton.vue';

  export default {
    name: "PostForm",
    components: { BaseInput, BaseButton },
  };
  
</script>
<style lang="scss">
.item {
  border: 2px solid #4C4352;
  border-radius: 5px;
  min-height: 100px;
  width: 100%;

  .header {
    background: #4C4352;
    height: 55px;
    border-radius: 3px;
    color: #fff;
    display: flex;
    align-items: center;
    justify-content: center;
    
    .title {
      font-weight: 900;
      font-size: 24px;
    }
  }

  .post-textarea {
    height: 300px;
    margin: 20px 5px 0 5px;
    width: 230px;
  }
}
</style>