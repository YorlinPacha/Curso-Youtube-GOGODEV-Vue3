<template>
    <div class="post">
        <h3>{{ props.title}}</h3>
        <p>{{ props.content }}</p>
        <!-- 1)activa la funcion que tiene el emit -->
        <button @click="handleClick">Activar emit</button>
        <!-- Agregar mas funcionalidades -->
        <input type="text" v-model="messega"/>
    </div>  
</template>

<script setup>
import { defineProps, defineEmits, ref } from 'vue';
//definimos las props
const props = defineProps({
    title: {
            type:String,
            required:true
        },
        content: {
            type:String,
            required:false,
            default: "No tienen contenido"
        },
})

//definimos los emits
const emit = defineEmits(['sayHi'])

const handleClick = () => {
            //comunicarnos con el componente padre
            //Funcion(evento) = msg
            emit("sayHi", messega.value)
        }
        let messega= ref("");

</script>



<!-- recibiremos los props de la forma tradicional Options-->
<!-- <script lang="ts">
import { defineComponent, ref } from 'vue';
export default defineComponent({
    name: 'PostDetail',
    //Aqui va el campo de props
    props:{
        title: {
            type:String,
            required:true
        },
        content: {
            type:String,
            required:false,
            default: "No tienen contenido"
        },
    },
    //emits que estamos recibiendo
    emits: [
        "sayHi"
    ],
    //Utilizar la informacion o las props que se reciben como argumentos
    //Emitimos eventos, recibir emits para utilizarlos y desestructuramos
    setup(props, {emit}){
        //2) emitir el evento sayHi y le pasa los parametros, ya el padre recibe
        const handleClick = () => {
            //comunicarnos con el componente padre
            //Funcion(evento) = msg
            emit("sayHi", messega.value)
        }
        let messega= ref("");

        return {props, handleClick, messega}
    }
})
</script> -->

<style scoped>
.post{
    width: 300px;
    height: 100px;
    border-radius:10px ;
    background-color: antiquewhite;
    margin: 10px;
    padding: 10px;
}

</style>