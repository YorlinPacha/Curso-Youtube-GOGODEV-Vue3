<template>
    <h1>Directiva V-Bind</h1>
  <p v-bind:class="{ 'danger' : hasError }">El mensaje se ha enviado correctamente</p>
</template>

<!-- Formato OPTIONS API -->
<script lang="ts">

</script>

<!-- Composition API -->
<!-- <script lang="ts">
    import { defineComponent } from 'vue';
    export default defineComponent({
        name: "ClassBind",
        setup(){
            let hasError = true;
            return {hasError}
        }
    })
</script> -->

<!-- con setup -->
    <!-- <script lang="ts" setup>
         let hasError = true;
    </script> -->

<style scoped>
.danger{
    color: red;
}
</style>