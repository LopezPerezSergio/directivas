<template>
    <!-- Conociendo las directivas de Seleccion -->
    <ExampleSelective />
    
    <!-- Conociendo las directivas de Recorrido -->
    <ExampleFor />

    <!-- Conociendo la directiva de V-Bind -->
    <ExampleVBind />

    <!-- Conociendo la directiva de eventos -->
    <ExampleEvent />
</template>

<script lang="ts" setup>
    import ExampleSelective from './components/ExampleSelective.vue'
    import ExampleFor from './components/ExampleFor.vue'
    import ExampleVBind from './components/ExampleVBind.vue'
    import ExampleEvent from './components/ExampleEvent.vue'
</script>

<style>
h1 {
  color: green;
}
</style>
