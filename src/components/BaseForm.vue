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
      <BaseTextarea placeholder="Post (máximo de 300 caracteres)" />
      <base-button @click.native="sendPost()">
        Criar novo post
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
        subtitle:''
      }
    },
    methods: {
      sendPost() {        
        console.log(this.title, this.subtitle);
      }
    },
    components: {BaseInput,BaseButton,BaseTextarea}
  }
</script>
<style></style>