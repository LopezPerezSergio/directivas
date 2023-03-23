<template>
    <!-- Directiva de eventos-->
    <p :style="{ color: color, backgroundColor: '#ccc' }">El mensaje se ha enviado satisfactoriamente</p>

    <button @click="handleClick()">Cambiar color</button>
</template>

<script lang="ts" setup>
    import {ref} from 'vue'
    
    let color = ref('#fff')

    const handleClick = () => {color.value = '#ff0000'}
</script>

<style scoped></style>
