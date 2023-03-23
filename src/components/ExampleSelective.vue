<template>
    <!-- Directiva de If else -->
    <h1 v-if="age < 18">Eres menor de edad</h1>
    <h1 v-else>Eres mayor de edad</h1>

    <!-- Directiva de show -->
    <h1 v-show="age < 18">Eres mas chica de edad</h1>
    <h1 v-show="age >= 18">Eres mas grande de edad</h1>

</template>

<script lang="ts" setup>
    let age = 10;
</script>

<style scoped>
</style>
