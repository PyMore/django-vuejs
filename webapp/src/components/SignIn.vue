<template>
  <div id="signin">
    <h2 id="header-mesaje">{{msg}}</h2>
    <form action="">
      <input type="text">
      <input type="password" name="" id="">
      <input type="button" value="Iniciar" v-on:click="start">
    </form>
  </div>

</template>

<script>
  'use strict';
  import axios from 'axios';

  export default {
  name: 'SignIn',
  data () {
    return {
      msg: 'Welcome to SignIn'
    }
  },

  methods:{
     start: function (event) {
       this.sing_in()
     },
    
    sing_in(){
      
      axios.get('https://pokeapi.co/api/v2/pokemon/')
      .then(function (response) {
        console.log(response);
      })

      .catch(function (error) {
        console.log(error);
      });

    }     

  }

}
</script>


<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

  input{
    width: 20em;
  }

  #header-mesaje{
    text-align: center;
    font-family: 'Avenir', Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    color: #2c3e50;
    
  }
  form{
    display: initial;
  }




</style>
