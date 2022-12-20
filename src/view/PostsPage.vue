<template>
  <div class="container">
    <!-- <div class="item posts">
      <div class="header">
        <span class="title">
          Posts
        </span>
      </div>
    </div> -->
    
    <PostView />
    <PostForm />
  </div>
</template>
<script>
import PostForm from '../components/PostForm.vue'
import PostView from '../components/PostView.vue'

export default {
  name: "PostsPage",
  components: { PostForm, PostView },
};

</script>
<style lang="scss">
.container {
  display: grid;
  grid-template-columns: 2fr 1fr;
  padding: 10px 20px;
  grid-column-gap: 17px;

}
</style>