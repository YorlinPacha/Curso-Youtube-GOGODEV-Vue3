<template>
    <div class="post">
        <h3>{{ props.title}}</h3>
        <p>{{ props.content }}</p>
    </div>  
</template>

<!-- recibiremos los props de la forma tradicional -->
<script lang="ts">
import { defineComponent } from 'vue';
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
    //Utilizar la informacion o las props que se reciben como argumentos
    setup(props){
        return {props}
    }
})
</script>

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