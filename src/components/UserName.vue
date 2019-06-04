<template>
  <div class="hello">
    <h1>Saludator 3000</h1>

    <label for="usernameinput">Ingrese nombre de usuario:</label>
    <br>
    <input id="usernameinput" type="text" v-model="theusername">


    <h3 
      v-if="theusername.length > 1" 
      v-bind:class="[colorClass]" >{{greeting}} {{ theusername }} </h3>
    

    <h3 v-if="theusername.length <= 0" >"ingresaa un nombre usuario"</h3>

    <button v-on:click="cambiarRojo">Cambiar a rojo</button>
    <button v-on:click="cambiarAzul">Cambiar a azul</button>

  </div>
</template>

<script>
export default {
  name: 'UserName',
  props: {
    greeting: String
  },
  data() {
    return {
      theusername: "zonawiki user",
      colorClass: "black"
    }
  },
  methods: {
    cambiarRojo: function (e) {
      this.colorClass = "rojo"
    },
    cambiarAzul: function (e) {
      this.colorClass = "azul"
    }
  }
}
</script>

<style>
  .rojo {
    color: red;
  }

  .azul {
    color: blue;
  }
</style>

