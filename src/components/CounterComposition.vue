<template>
  <h1>Composition {{ counter }}</h1>
  <button @click="addCounter">Incrementar</button>
</template>

<script lang="ts" setup>
//en vez de aplicar opciones (option), con setup = se va a encargar de realizar las accionde de
//datos necesarios, definir los metodos o funciones. el formato esstara 
//mas orientado al uso de hooks (ciclos de vida del componente)

// con composition tenemos mas control de REACTIVIDAD

import { ref } from 'vue';
let counter = ref(0);
const addCounter = () =>{
    counter.value++
}
</script>

<style>

</style>