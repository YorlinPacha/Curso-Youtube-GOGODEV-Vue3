<template>
  <div class="post-card">
    <h3>Titulo</h3>
    <p>Lorem, ipsum dolor sit amet consectetur adipisicing elit. Velit libero cupiditate animi! Numquam velit fugit eius porro officiis quaerat. Rerum totam veniam necessitatibus facilis impedit ratione excepturi ab voluptatibus reiciendis!</p>
    <PostButton/>
  </div>
</template>

<script lang="ts" setup>
import PostButton from './PostButton.vue';

</script>

<style scoped>
.post-card{
    border-radius: 15px;
    padding:  10px;
    margin: 5px;
    border: 1px solid #ccc;
}
</style>