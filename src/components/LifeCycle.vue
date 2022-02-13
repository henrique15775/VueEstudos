<template>
  <h1> Meu Nome é: {{ nome }}</h1>  
</template>


<script>

export default {
  name:"LifeCycle",
  data(){
    return {
      nome: "Ainda n sei"
    }
  },
  created(){
    setTimeout(()=>{
      this.nome = "Matheus"
    },1000);
  },
  mounted(){
      setTimeout(()=>{
      this.nome = "Henrique"
    },2000);
  }
}
</script>
