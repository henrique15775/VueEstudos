<template>
  <img :src="avatar" :alt="descricao">
</template>


<script>
export default{
  name: "Picture",
  data(){
    return{
      avatar: "/favicon.ico",
      descricao: "Henrique"
    }
  }
}
</script>