<script setup>
  const name = 'Vue dinamico'
  const estiloColor = "color:blue"
  const arrayColor = ["blue" , "red" , "Mexico"]
  const activo = true;
</script>


<template>
  <h1>Hola {{ name.toUpperCase() }}</h1>
  <h2>{{ arrayColor }}</h2>
  <h2 :style="'color: ${arrayColor[2]}'">Soy mexicano</h2>
  <h2 v-if="activo === true">Estoy activo</h2>
  <p v-else-if="activo === false">Estoy desactivo</p>
  <p v-else>Estoy indeciso</p>
</template>


<style scoped>
  h1{
    color: red;
  }
</style>