<template>
<div>

  <HelloWorld />
  <LifeCycle />
  <Pessoa />
  <Form />
  <Picture />
  <Header />
</div>
  
  </template>


<script>
  import HelloWorld from './components/HelloWorld.vue'
  import LifeCycle from './components/LifeCycle.vue'
  import Pessoa from './components/Pessoa.vue'
  import Form from './components/Form.vue'
  import Picture from './components/Picture.vue'
  import Header from './components/Header.vue'
  export default {
    name: 'App',
    components: {
      HelloWorld,
      LifeCycle,
      Pessoa,
      Form,
      Picture,
      Header
    }
  }
</script>

<style>
  body{
    color: white;
    background-color: #333;
  }
  a{
    color:red;
  }
 
</style>