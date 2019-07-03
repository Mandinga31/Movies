<template>
  <div id="app">
    <h1>{{ Titulo }}</h1>
    <img alt="Vue logo" src="./assets/logo.png">
    <HelloWorld v-bind:msg="titulo"/>
    <form class="form-inline" v-on:submit.prevent ="miMetodo">
    </form>
  </div>
</template> 

<script>
import Navbar from './components/Navbar.vue'
import Content from './components/Content.vue'
import { Script } from 'vm';

export default {
  name: 'app',
  components: {
    Navbar,
    Content
  },
  data(){
    return {
     MovieTitleToSearch:''
    }
    },
    
    methods:{
      searchMovie: function (title) {
          this.movieTitleToSearch = title
            } 
}
}
</script>