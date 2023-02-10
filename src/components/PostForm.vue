<template>
  <div>
    <form @submit.prevent>
      <BaseInput
        v-model="title"
        placeholder="Título" 
      />
      <BaseInput
        v-model="subtitle"
        placeholder="Sub-título"
      />
      <BaseTextarea
        v-model="content"
        placeholder="Post (máximo de 300 caracteres)"
      />
      <base-button        
        @click.native="sendPost()"
      >
        <span class="btn-primary-text">Criar novo post</span>
      </base-button>
    </form>
  </div>
</template>
<script>
  import BaseInput from './BaseInput.vue';
  import BaseButton from './BaseButton.vue';
  import BaseTextarea from './BaseTextarea.vue';

  export default{
    data() {
      return {
        title: '',
        subtitle:'',
        content: ''
      }
    },
    methods: {
      sendPost() {        
        console.log(this.title, this.subtitle, this.content);
      }
    },
    components: {BaseInput,BaseButton,BaseTextarea}
  }
</script>
<style lang="scss">
.btn-primary-text {
  background: #961EF4;
  background: linear-gradient(to right, #961EF4 0%, #E35858 100%);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  font-size: 12px;
  line-height: 15px;
  font-weight: 700;
}
</style>