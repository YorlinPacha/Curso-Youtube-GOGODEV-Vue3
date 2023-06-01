<template>
<!-- pintar datos del componente en la vista usamos {{  }} -->
  <h1>Option {{ counter }}</h1>
  <button @click="addCounter">Incrementar</button>
</template>

<script lang="ts">
//importar para definir nuestros componentes => defineComponent
import { defineComponent } from 'vue';
//exportar la definicion de nuestro componente para que pueda ser usada
//Recibira un objeto que define el componente
export default defineComponent({
    //le damos nombre al componente
    name: "CounterOption",
    //si usamos componentes dentro de nuestro componente, tocaria escribirlos e importarlos
    // components: {MiComponente1,MiComponente2}
    // como no usamos, estara vacio
    //components: {}, se quita porque no se usa
    //definir los datos que vamos a usar, variables, elementos vamos que a tener
    // en nuestro componente, con DATA, funcion que retorna datos
    data(){
        let counter = 0;
        //se retorna un obj con todas las variables
        return {counter}
    },
    //Utilizar los metodos
    methods:{
        addCounter(){
            //nos referimos a los datos
            this.counter++
        }
       //Otros metodos... 
    }
})
</script>

<style scoped>

</style>