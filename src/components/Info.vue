<template>
  <div>

    <p v-if="esta_trabalhando">Estou trabalhando no momento.</p>
    <p v-else>Estou em busca de novas oportunidades</p>
    <ul>
      <li>Javascript</li>
      <li>PHP</li>
      <li>Python</li>
    </ul>
    <p v-if="1<2">1 É MENOR Q 2</p>
    <p v-show="mostrar_email"> O email é: {{ email }} </p>
</div>
</template>

<script >
 export default {
   name: "Info",
   data() {
     return {
       esta_trabalhando: false,
       mostrar_email: true,
       email: "123@gmail.com"
     }
   }
 }
</script>
