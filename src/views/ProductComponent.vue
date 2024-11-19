<script setup>
import productos from '@/assets/productos.json'

</script>

<template>
    <div>
        <div>
            <p>{{ productos[$route.params.id-1].name }}</p>
            <p>{{ productos[$route.params.id-1].description }}</p>
        </div>
    </div>
</template>

<style scoped>
</style>