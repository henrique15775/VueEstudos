<template>
<div>

  <HelloWorld />
  <LifeCycle />
  <Pessoa />
  <Form />
</div>
  
  </template>


<script>
  import HelloWorld from './components/HelloWorld.vue'
  import LifeCycle from './components/LifeCycle.vue'
  import Pessoa from './components/Pessoa.vue'
  import Form from './components/Form.vue'

  export default {
    name: 'App',
    components: {
      HelloWorld,
      LifeCycle,
      Pessoa,
      Form
    }
  }
</script>