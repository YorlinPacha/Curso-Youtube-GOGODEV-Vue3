<template>
  <h1>Lista de paises FOR</h1>
  <p>Acceder a un Array</p>
  <ul>
    <li v-for="(country, index) in countries" v-bind:key="index">{{ country }}</li>
  </ul>
  <!-- Accedemos a los objetos -->
  <p>Acceder a Objetos</p>
  <ul>
    <li v-for="countryObj in countriesObj" v-bind:key="countryObj.code">{{ countryObj.name }}</li>
  </ul>
</template>

<script lang="ts" setup>
// Ref = solo es necesario para typestcript
import { Ref, ref } from 'vue';
// :Ref<Array<string>>  => solo por typescript, si no se quita
let countries:Ref<Array<string>> = ref([
    "Spain", "Italy", "Portugal", " UK"
])

//Ahora lo haremos con objetos - comsumo de APIS
let countriesObj= ref([
    {
        code: "es",
        name:"Spain"
    },
    {
        code: "en",
        name:"UK"
    },
    {
        code: "fr",
        name:"France"
    },
    {
        code: "it",
        name:"Italy"
    },
    {
        code: "pt",
        name:"Portugal"
    },
])

</script>

<style scoped>

</style>