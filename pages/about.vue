<template>
    <div>

        <h2 class="text-4xl">About page</h2><br>
        <p>Hello this is a paragraph in about</p>
        <p v-bind="source">Lorem ipsum dolor, sit amet consectetur adipisicing elit. Nostrum quibusdam quaerat laudantium! Consequatur harum ratione veniam rem temporibus tenetur optio eum repellendus quo fuga. Facilis aspernatur similique quod natus labore!</p>
        <br>
        <NuxtLink to="/" style="color:#12b488"><b>Home Link</b></NuxtLink> <br/>
        <a href="/">home page anchor</a>
    </div>
</template>

<script setup>

</script>



<style scoped>

</style>