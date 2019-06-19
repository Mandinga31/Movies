<template>
  <div id="app">
    <Navbar/>
    <h1>{{ Titulo }}</h1>
    <img alt="Vue logo" src="./assets/logo.png">
    
  </div>
</template>

<script>
import NavBar from './components/Navbar.vue'
//import content from './components/NavBar.vue'

export default {
  
  name: 'app',
  components: {
    Navbar
  },
  data() {
    return {
      titulo:"proyecto vue cli"
    } 
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
