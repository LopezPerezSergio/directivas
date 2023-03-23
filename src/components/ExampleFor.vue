<template>
    <!-- Directiva For para recorrer el array-->
    <!-- Directiva v-bind:key para dar un identidicador unico tambien se puede escribir :key="valor" -->
    <ul>
        <li v-for="country in countries" :key="country.code">{{ country }}</li>
    </ul>

    <ul>
        <li v-for="country in objectsCountries" :key="country">{{ country.name }}</li>
    </ul>
</template>

<script lang="ts" setup>
    import {Ref, ref} from 'vue'

    interface ICountry{
        code: string,
        name: string
    }

    let countries:Ref<Array<string>> = ref([
        'Spain', 'France', 'UK', 'Italy', 'Portugal'
    ])

    let objectsCountries:Ref<Array<ICountry>> = ref([
        {
            code:'es',
            name:'Spain'
        },
        {
            code:'fr',
            name:'France'
        },
        {
            code:'en',
            name:'UK'
        },
        {
            code:'it',
            name:'Italy'
        },
        
        {
            code:'pt',
            name:'Portugal'
        },
    ])
</script>

<style scoped>
</style>
