<template>
  <h1>Listado</h1>
  <hr>
  <CounterOption/>
  <hr>
  <CounterComposition/>
  <hr>
  <PostContainer/>
  <hr>
  <h2>Directivas selectivas</h2>
  <ExampleSelectiveVue />
  <hr>
  <h2>Directiva v-for</h2>
  <ExampleFor />
  <hr>
  <h2>Class v-bind</h2>
  <ClassBind />
  <hr>
  <h2>Model form v-model</h2>
  <ModelForm />
  <hr>
  <h2>Ciclo de vida con options api</h2>
  <CycleOption />
  <hr>
  <h2>Ciclo de vida con Composition api</h2>
  <CycleCompositionApi />
  <hr>
  <hr>
  <h2>Post para Pros y emit</h2>
  <PostList />
  <hr>
  <h2>Ejemplo Datos computados</h2>
  <ComputedExample />
  <hr>
  <h2>Ejercicio computados</h2>
  <ComputedExampleEjercicio />
  <hr>
</template>

<script lang="ts" setup>
import PostContainer from './components/PostContainer.vue';
import CounterOption from './components/CounterOption.vue';
import CounterComposition from './components/CounterComposition.vue';
import ExampleSelectiveVue from './components/ExampleSelective.vue';
import ExampleFor from './components/ExampleFor.vue';
import ClassBind from './components/ClassBind.vue';
import ModelForm from './components/ModelForm.vue';
import CycleOption from './components/CycleOption.vue';
import CycleCompositionApi from './components/CycleCompositionApi.vue';
import PostList from './components/PostList.vue'
import ComputedExample from './components/ComputedExample.vue';
import ComputedExampleEjercicio from './components/ComputedExampleEjercicio.vue';
</script>

<style scoped>
/* estilos generales */
  h1{
    color: blue;
  }
  h2{
    color: green;
  }
  hr {
  border-color: red;
}
</style>
