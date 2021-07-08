<template>
  <div>
    <h1> Esta es mi informacion: {{ informacion }}</h1>
    <input type="text" v-model="informacion" />
  </div>
</template>

<script>
export default {
  data() {
    return {
      informacion: "",
    };
  },
};
</script>
