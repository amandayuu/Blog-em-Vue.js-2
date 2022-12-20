<template>
<div>
  <div class="item posts">
      <div class="header">
        <span class="title">
          Posts
        </span>
      </div>
    </div>
</div>
</template>
<script>
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
}
</style>