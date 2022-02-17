<template>
  <div>

    <p v-if="esta_trabalhando">Estou trabalhando no momento.</p>
    <p v-else>Estou em busca de novas oportunidades</p>
    <ul >
      <li v-for="(tech, index) in backend_technologies" v-bind:key="index"> {{ tech }} </li>
    </ul>
    <ul>
      <li v-for="tech in frontend_technologies" v-bind:key="tech.id"> {{ tech.nome }}</li>
    </ul>
    <p v-if="1<2">1 É MENOR Q 2</p>
  <div>
    <button @click="showEmail">Clica</button>
  </div>
    <p v-show="mostrar_email"> O email é: {{ email }} </p>
    <p>Link Google -> <a v-bind:href="meu_link" target="_blank">Basta Clicar aqui</a></p>
</div>
</template>

<script >
 export default {
   name: "Info",
   data() {
     return {
       esta_trabalhando: false,
       mostrar_email: false,
       email: "123@gmail.com",
       meu_link: "https://google.com",
       backend_technologies:["Javascript","PHP","Python"],
       frontend_technologies:[
         {
           id:1,
           nome:"HTML"
       },{
          id:2,
          nome:"CSS"
       },{
          id:3,
          nome:"Javascript"
       }]
     }
   },
   methods:{
     showEmail(){
       this.mostrar_email = !this.mostrar_email
     }
   }
 }
</script>
