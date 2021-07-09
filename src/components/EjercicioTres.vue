<template>
    <div>
        <h2  :class="[{'bg-primary': cambio, 'bg-danger': !cambio}, color]">Prueba diferentes colores para tu texto</h2>
        <input type="text" v-model="color">
        <button class="btn" @click="cambio = !cambio" >Cambiar</button>
    </div>
</template>


<script>
export default {
    data () {
        return {
            color: "",
            cambio: true
        }
    },
}
</script>

<style>
  
</style>