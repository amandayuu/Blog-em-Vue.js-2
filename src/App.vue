<template>
  <div id="app">
    <PostsPage />
  </div>
</template>

<script>
import PostsPage from "./view/PostsPage.vue"
export default {
  name: 'App',
  components: {
    PostsPage
  }
}
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
