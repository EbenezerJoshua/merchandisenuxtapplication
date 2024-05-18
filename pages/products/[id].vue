<template>
    <div>
        <h2>Product detials for <b>{{ product.title }}</b></h2>
        <p>The price is <b>${{ product.price }}</b> </p>
        <p>The id is {{ product.id }} (you can see in the URL) </p>
    </div>
</template>

<script setup>
    const {id} = useRoute().params
    const uri = 'https://fakestoreapi.com/products/' + id

    // fetch the product

    const { data: product } = await useFetch(uri, { key: id })

    definePageMeta({
        layout: 'products'
    })
</script>

<style scoped>

</style>
