<template>   
  <BaseComponentes/>  
</template>

<script>
import BaseComponentes from './baseview/BaseComponentes.vue'


export default {
  name: 'App',
  components: {    
    BaseComponentes,    
  }
}
</script>

<style>
html{
 background: rgb(1,27,40);  
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #fff;
  margin: 0px;
  padding: 0px;  
  background: rgb(1,27,40);   
}
</style>
