<template>
  <h1>Hola Mundo</h1>  
</template>

<script lang="ts">
import { defineComponent } from 'vue';

export default defineComponent({
    name: "CycleOption",
    data(){
        //Estara vacio, se puede eliminar
    },
    methods:{

    },
    //Añadiendo los ciclos de vida Y SE EJECUTAN EN ORDEN
    created(){
        console.log("Created");
    },
    mounted(){
        console.log("mounted");
    },
    updated(){
        console.log("updated");
    },
    unmounted(){
        console.log("unmounted");
    }
})
</script>

<style scoped>

</style>