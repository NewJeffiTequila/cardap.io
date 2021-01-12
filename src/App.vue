<template>
  <div id="app">
    <div class="d-flex justify-content-center mb-3">
      <img src="@/assets/hamburger-solid.svg" alt="" width="60">
      <h1 class="display-4">CARDAP.IO</h1>
    </div>
    <RestaurenteCardapio/>

  </div>
</template>

<script>
// import TelaCardapio fro/m './components/TelaCardapio.vue'
import RestaurenteCardapio from './components/RestaurenteCardapio.vue'

export default {
  name: 'App',
  components: {
    RestaurenteCardapio
  }
}
</script>

<style>
/* #app { */
  /* font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px; */
/* } */
</style>
