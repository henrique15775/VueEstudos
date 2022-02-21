<template>
  <ul>
    <li>A1</li>
     <li>A1</li>
      <li>A1</li>
       <li>A1</li>
       <li v-if="esta_logado"> <a href="#" > Meu Perfil </a></li>
  </ul>
</template>
<style scoped>
  ul{
    list-style: none;
    display:flex;
  }
</style>
<script>
  export default {
    name: 'Header',
    props: ["esta_logado"]
  }
</script>