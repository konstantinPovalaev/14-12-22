<template>
  <img alt="Vue logo" src="./assets/logo.png">
  <HelloWorld msg="Welcome to Your Vue.js App" :name="name" :phone="phone" :photo="photo"/>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'

export default {
  name: 'App',
  components: {
    HelloWorld,
  },
  one(){
    name  "",
    phone "",
    photo ""
  },
  two(){
    this.axios.get('https://randomuser.me/api/')         
    .then((response) => {
      console.log(response.data),
      this.name = "kosty" 
      this.phone = "89295856468" 
      this.photo ="aa"    
    }) 
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
