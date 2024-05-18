
<template>
    <div class="card text-center">
        <img :src="product.image" alt="product thumb" class="thumb">
        <p class="font-bold text-grey-500 m-4 truncate">{{ product.title }}</p>
        <p class="font-bold text-black-500 m-4 truncate">${{ product.price }}</p>
        <NuxtLink :to="`/products/${product.id}`"> 
            <p class="btn my-4">View detials</p>
            <!-- {{ product.title }} -->
        </NuxtLink>

    </div>
</template>

<script setup>
    const { product } = defineProps(['product'])
</script>
    
<style scoped>

</style>