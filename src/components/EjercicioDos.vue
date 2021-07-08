<template>
  <div class="EjercicioDos">
    <input class="EjercicioDos__input" type="text" v-model.number="numeroUno" />
    <input class="EjercicioDos__input" type="text" v-model.number="numeroDos" />
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

<style>
.EjercicioDos{
  margin-top: 50px;
}

.EjercicioDos__input{
 background: rgb(61, 198, 223); 
 color: rgb(219, 37, 128);
}

</style>
