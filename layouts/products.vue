<template>
    <div>
        <header class="shadow-sm bg-white">
            <nav class="container mx-auto p-4 flex justify-between">
                <NuxtLink to="/" class="font-bold">Brand Name</NuxtLink>
                <NuxtLink to="/products" class="font-bold">Merchandise</NuxtLink>
                <ul class="flex gap-10">
                    <li><NuxtLink to="/">Home</NuxtLink></li>
                    <li><NuxtLink to="/products">Products</NuxtLink></li>
                    <li><NuxtLink to="/about">About</NuxtLink></li>
                </ul>
            </nav>
        </header>
        <div class="container mx-auto p-4">
            <slot/>
        </div>
    </div>
    <footer class="container mx-auto p-4 flex justify-between border-t-2">
        <ul class="flex gap-4">
            <!--We use nuxtlink instead of anchor tag because a-tag fetched data from the server and loads locally but this nuxt link loads website in server and it sends back to us
            omvopzmdsfvpomdpfv-->
            <li><NuxtLink to="/">Home</NuxtLink></li>
            <li><NuxtLink to="/products">Product Index</NuxtLink></li>
            <li><NuxtLink to="/about">About</NuxtLink></li>
        </ul>
    </footer>
</template>

<style>
    .router-link-exact-active{
        color: #12b488;
    }
</style>