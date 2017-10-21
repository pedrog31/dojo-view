<template>
  <div>
    <h2>home</h2>
      <input v-model= "message" placeholder="edit" name = "entrada">
      <button v-on:click="myFunction">Boton</button>
      <h1> {{texto}} </h1>
  </div>
</template>

<script>
export default {
  data () {
    return {
      message: "",
      texto: ""
  }
},
  methods: {
    myFunction () {
      this.texto = this.message
    }
}
}

</script>

<style>
</style>
