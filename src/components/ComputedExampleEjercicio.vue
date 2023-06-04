<template> 
<h2>Porcentajes de impuestos pagados</h2>
  <div>
    <label> subtotal </label>
    <input type="number" v-model="subtotal" />
    <h3>Total impuestos a pagar: {{ totalVat }} ({{ vat }}%)</h3>
  </div>
</template>

<script lang="ts" setup>
import { computed, ref } from 'vue';
// 21%
 const vat = 21
 let subtotal = ref(0);
 //Impuestos a pagar
 const totalVat = computed(()=> (vat*subtotal.value) / 100 )

 /* 
 100 --------- subtotal
 21 ---------- x
 x= (21 * subtotal) / 100
 
 */


</script>


<style scoped>

</style>