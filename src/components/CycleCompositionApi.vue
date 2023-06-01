<template>
  <h1>Hola Mundo</h1>
</template>

<script lang="ts" setup>
import { onMounted, onUpdated } from 'vue';

//Cuando el elemento es montado, algo ocurrira
onMounted(() => {
    console.log("mounted Composition")
})

onUpdated(() => {
    console.log("onUpdated Composition")
})


</script>

<style scoped></style>
