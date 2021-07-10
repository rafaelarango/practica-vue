<template>
  <div id="app" class="container">
    <img alt="Vue logo" src="./assets/logo.png">
    <EjercicioUno/>
    <EjercicioDos/>
    <EjercicioTres/>
    <EjercicioCuatro/>
  </div>
</template>

<script>
import EjercicioUno from  './components/EjercicioUno.vue';
import EjercicioDos from  './components/EjercicioDos.vue';
import EjercicioTres from './components/EjercicioTres.vue';
import EjercicioCuatro from './components/EjercicioCuatro.vue';

export default {
  components: {
    EjercicioUno,
    EjercicioDos,
    EjercicioTres,
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
