<template>
  <img :src="avatar" :alt="descricao">
  <MudarImagem @mudar-Imagem="trocarImagem" />
</template>


<script>
 import MudarImagem from './MudarImagem.vue'
export default{
  name: "Picture",
  data(){
    return{
      avatar: "/favicon.ico",
      descricao: "Henrique"
    }
  },components: {
    MudarImagem
  },
  methods:{
    trocarImagem(){
      this.avatar = './reactLogo.jfif';
    }
  }
}
</script>