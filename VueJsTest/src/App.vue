<template>
  <div id="app">    
    <router-view/>
  </div>
</template>

<script>
export default {
  name: 'App'
}
</script>

<style>
body{
  background: rgb(0,23,33);
  background: linear-gradient(0deg, rgba(0,23,33,1) 0%, rgba(0,38,55,1) 100%);
}

#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #fff;
  margin-top: 60px;  
}

</style>
