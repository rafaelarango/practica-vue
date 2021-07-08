<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <EjercicioUno/>
    <EjercicioDos/>
  </div>
</template>

<script>
import EjercicioUno from  './components/EjercicioUno.vue';
import EjercicioDos from  './components/EjercicioDos.vue';

export default {
  components: {
    EjercicioUno,
    EjercicioDos
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

div{
  margin-top: 50px;
}

.EjercicioDos input{
 background: rgb(61, 198, 223); 
 color: rgb(219, 37, 128);
}

</style>
