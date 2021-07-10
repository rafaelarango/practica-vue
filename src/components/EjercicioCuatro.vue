<template>
  <div>
    <h2>{{ titulo }}</h2>
    <h3>{{ texto }}</h3>
    <div class="d-flex justify-content-center">
      <button class="btn btn-primary mb-3 me-3" @click="estado = !estado">
        true - false
      </button>
      <button class="btn btn-warning mb-3" @click="mostrar = !mostrar">
        Todos los estudiantes
      </button>
    </div>

    <P v-for="estudiante of estudiantes" :key="estudiante">
      <span v-if="mostrar === false">
        {{ estudiante.nombre }} {{ estudiante.apellido }}. Estado:
        {{ estudiante.activo }}</span
      >
      <span v-if="mostrar === true && estudiante.activo === estado">
        {{ estudiante.nombre }} {{ estudiante.apellido }}. Estado:
        {{ estudiante.activo }}</span
      >
    </P>
  </div>
</template>

<script>
export default {
  data() {
    return {
      titulo: "Hola mundo Vue",
      texto: "Estos son los mejores estudiastes de Vue CLI 2021",
      estudiantes: [
        { nombre: "Migue", apellido: "Silver", activo: true },
        { nombre: "Flor", apellido: "Gomez", activo: false },
        { nombre: "Carlos", apellido: "Eduardo", activo: true },
        { nombre: "Andres", apellido: "Medina", activo: false },
        { nombre: "Andres", apellido: "Calle", activo: true },
        { nombre: "Sara", apellido: "Tamallo", activo: false },
        { nombre: "Mabael", apellido: "Ramirez", activo: true },
        { nombre: "Yuli", apellido: "Henao", activo: true },
        { nombre: "Rafael", apellido: "Arango", activo: true },
        { nombre: "Luis", apellido: "Perez", activo: false },
      ],
      estado: true,
      mostrar: false,
    };
  },
};
</script>
