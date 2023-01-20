<template>
  <div class="container">
    <BaseForm />
  </div>
</template>
<script>
import BaseForm from '@/components/BaseForm.vue';
export default {
  name: "PostsPage",
  components: {
    BaseForm
  }
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