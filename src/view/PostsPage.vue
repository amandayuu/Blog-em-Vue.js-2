<template>
  <div class="container">
    <div class="card" />
    <PostForm class="card" />
  </div>
</template>
<script>
import PostForm from '@/components/PostForm.vue';
export default {
  name: "PostsPage",
  components: {
    PostForm
  }
};

</script>
<style lang="scss">
.container {
  display: grid;
  grid-template-columns: 2fr 1fr;
  padding: 10px 20px;
  grid-column-gap: 17px;

  .card {
    border: 2px solid #4C4352;
    border-radius: 5px;
  }

}
</style>