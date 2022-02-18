<template>
  <img :src="avatar" :alt="descricao">
  <MudarImagem @mudar-Imagem="mudarImagem" />
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

    }
  }
}
</script>