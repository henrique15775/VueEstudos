<template>
<div>

  <HelloWorld />
  <LifeCycle />
  <Pessoa />
  <Form />
  <Picture />
</div>
  
  </template>


<script>
  import HelloWorld from './components/HelloWorld.vue'
  import LifeCycle from './components/LifeCycle.vue'
  import Pessoa from './components/Pessoa.vue'
  import Form from './components/Form.vue'
  import Picture from './components/Picture.vue'

  export default {
    name: 'App',
    components: {
      HelloWorld,
      LifeCycle,
      Pessoa,
      Form,
      Picture
    }
  }
</script>