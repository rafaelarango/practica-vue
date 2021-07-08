<template>
  <div class="EjercicioDos">
    <input type="text" v-model.number="numeroUno" />
    <input type="text" v-model.number="numeroDos" />
    <h4>Total: {{ sumarNumeros }}</h4>
  </div>
</template>

<script>
export default {
  data() {
    return {
      numeroUno: 0,
      numeroDos: 0,
    };
  },

  computed: {
    sumarNumeros() {
      return this.numeroUno + this.numeroDos;
    },
  },
};
</script>
