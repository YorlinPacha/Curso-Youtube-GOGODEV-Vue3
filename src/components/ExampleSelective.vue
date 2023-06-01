<!-- Renderizados selecctivos / Directivas -->
<template>
  <h1>Directiva selectiva</h1>
  <h2 v-if="age < 18">Eres menor de edad</h2>
  <h2 v-show="age >= 18">Eres mayor de edad</h2>
</template>

<!-- composition API setup -->
<script lang="ts" setup>
    let age = 18;
</script>



<!-- composition API setup (largo) -->
<!-- <script lang="ts">
import { defineComponent } from 'vue';
export default defineComponent({
    name: "ExampleSelective",
    setup(){
        let age = 10;
        return {age}
    }
})    
    
</script> -->

<style scoped>

</style>