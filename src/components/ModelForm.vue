<template>
  <h1>Model Form V-model (input, checkbox, select)</h1>
  <form>
    <input type="text" v-model="inputText" />
    <input type="checkbox" v-model="agree"/> Aceptar termino y condiciones
  <select v-model="country">
    <option value="Elige...">Elige...</option>
    <option value="Colombia">Colombia</option>
    <option value="HK">HK</option>
    <option value="China">China</option>
  </select>
</form>
  <h3> {{ inputText }}</h3>
</template>

<!-- OPTION API -->
<!-- <script lang="ts">
import { ref, defineComponent } from 'vue';

export default defineComponent({
    data(){
        return { 
            inputText: "", 
            agree: true
    }
    }
})

</script> -->

<!-- ++++++++++++++++++++++++++++++++++++++++++++++++++++++ -->

<!-- COMPOSITION API -->
<script lang="ts" setup>
//Obtendremos el valor del input y tenerla actualizada
//estaran vinculados

import { ref } from 'vue';
let inputText = ref("");
let agree = ref(true);
let country = ref("Elige...")

</script>

<!-- ++++++++++++++++++++++++++++++++++++++++++++++++++++++ -->

<!-- METODO STANDARD COMPOSITION API -->
<!-- <script lang="ts">
import { ref, defineComponent } from 'vue';

export default defineComponent({
    setup() {
        let inputText = ref("")
        return {inputText}
    }
})
</script>  -->


<style scoped>

</style>