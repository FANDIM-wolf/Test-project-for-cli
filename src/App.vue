<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <Mycomponent/>
   
  </div>
</template>

<script>
import Mycomponent from './components/Mycomponent'
export default {
  name: 'App',
  
  components: {
    Mycomponent
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
