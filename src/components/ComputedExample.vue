<template> 
  <div>
    <input type="text" v-model="message">
    <h3> {{ message }}</h3>
    <h3>{{ reverse }}</h3>
  </div>
</template>

<!-- iniciamos con OPTION API -->
<!-- <script lang="ts">
import { defineComponent } from 'vue';

export default defineComponent({
    name: 'ComputedExample',
    data(){
        return{
            message: ''
        }
    },
    computed:{
        //Variable que realizara algun calculo antes de devolverla
        //En este caso modifica message
        reverse(){
            return this.message.split('').reverse().join('')
        }
    }
})

</script> -->

<!-- COMPUTED EN COMPOSITION API -->
<!-- <script lang="ts">
import { defineComponent, ref, computed } from 'vue';

export default defineComponent({
    name: 'ComputedExample',
    setup(){
        let message = ref("")
        const reverse = computed(()=> message.value.split('').reverse().join(''))
        return { message, reverse}
    }
})

</script> -->

<!-- COMPUTED EN COMPOSITION API CORTA-->
<script lang="ts" setup>
import {ref, computed } from 'vue';

    let message = ref("")
    const reverse = computed(()=> message.value.split('').reverse().join(''))

</script>


<style scoped>

</style>