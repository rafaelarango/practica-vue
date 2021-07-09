<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <EjercicioUno/>
    <EjercicioDos/>
    <EjercicioCuatro/>
  </div>
</template>

<script>
import EjercicioUno from  './components/EjercicioUno.vue';
import EjercicioDos from  './components/EjercicioDos.vue';
import EjercicioCuatro from './components/EjercicioCuatro.vue';

export default {
  components: {
    EjercicioUno,
    EjercicioDos,
    EjercicioCuatro
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
