<template>
  <form @submit="enviarFomulario($event)">
   <div>
     <input type="text" v-model="nome" >
   </div>
   <div>
     <input type="text" v-model="email" >
   </div>
    <Submit />
  </form>
</template>


<script>
  import InputText from './form/InputText.vue'
  import Submit from './form/Submit.vue'
  export default{
    name:"Form",
    components:{
      InputText,
      Submit
    },data(){
      return {
        nome: "",
        email:""
      }
    },
    methods:{
      enviarFomulario(e){
        e.preventDefault()
        const name = this.nome;
        const email = this.email;

        window.alert(`Nome = ${name}\n Email = ${email}`)
      }
    }
  }
</script>