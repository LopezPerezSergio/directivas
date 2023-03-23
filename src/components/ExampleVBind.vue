<template>
    <p :class="{'danger':hasError}">El mensaje se ha enviado satisfactoriamente</p>

    <p :style="{color: 'red', backgroundColor: 'blue'}">El mensaje se ha enviado satisfactoriamente</p>
</template>

<script lang="ts" setup>
    let hasError = true;
</script>

<style>
    .danger{
        color:red;
    }
    
</style>
