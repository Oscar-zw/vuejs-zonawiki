<template>
  <div class="hello">
    <h1>Saludator 3000</h1>

    <label for="usernameinput">Ingrese nombre de usuario:</label>
    <br>
    <input id="usernameinput" type="text" v-model="theusername">

    <h3>{{greeting}} {{ theusername }} </h3>

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
      theusername: "zonawiki user"
    }
  }
}
</script>

