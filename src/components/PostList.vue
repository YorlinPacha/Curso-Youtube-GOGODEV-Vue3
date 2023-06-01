<template>
  <h1>Componente List padre</h1>  
  <div class="container">
    <!-- // recorrido con for y envio de datos con props -->
    <PostDetail v-for="elm in info" :key="elm.title" :title="elm.title" :content="elm.content"/>
</div>
</template>

<script lang="ts" setup>
import PostDetail from './PostDetail.vue';
let info = [
    {
        title:" Este post 1",
        content:"Texto de ejemplo1"
    },
    {
        
        title:" Este post 2",
        content:"Texto de ejemplo2"
    },
    {
        title:" Este post 3",
        content:"Texto de ejemplo3"
    },
    {
        
        title:" Este post 4",
        content:"Texto de ejemplo4"
    },
    {
        
        title:" Este post 5",
        content:"Texto de ejemplo5"
    }]
</script>

<style scoped>
.container{
    display: flex;
    flex-wrap: wrap;
    flex-direction: row;
    justify-content: space-around;

}
</style>