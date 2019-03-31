<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <HelloWorld msg="Vue.js Zonawiki"/>
    <UserName greeting="Hola Hubo "></UserName>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import UserName from './components/UserName.vue'


export default {
  name: 'app',
  components: {
    HelloWorld,
    UserName
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
