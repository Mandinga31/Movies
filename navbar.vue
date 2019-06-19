<template>
  <div id="app">
    <h1>{{ Titulo }}</h1>
    <img alt="Vue logo" src="./assets/logo.png">
    <HelloWorld v-bind:msg="titulo"/>
  </div>
</template> 

<script>
import HelloWorld from './components/HelloWorld.vue'

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
