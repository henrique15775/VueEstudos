<template>
<div>

  <HelloWorld />
  <LifeCycle />
</div>
  
  </template>


<script>
  import HelloWorld from './components/HelloWorld.vue'
  import LifeCycle from './components/LifeCycle.vue'

  export default {
    name: 'App',
    components: {
      HelloWorld,
      LifeCycle
    }
  }
</script>