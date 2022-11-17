<script setup>
import {RouterLink, RouterView} from 'vue-router'
</script>

<template>
  <img class="h-full w-full m-0 p-0 object-cover absolute bg-cover" src="./assets/WhatsApp Image 2022-09-30 at 10.11 1.png" alt="">
<div class="flex py-20 bg-transparent p-0 m-0 box-border">
<nav class="relative p-4 md:flex md:justify-end md:items-end md:space-x-10 text-white border-white border-2 w-full border-r-0 border-l-0 pr-10">
        <RouterLink class="flex gap-10" to="/"><img src="./assets/IdealMark 2.png" alt=""></RouterLink>
       <RouterLink to="/">Home</RouterLink>
        <RouterLink to="/about">About Us</RouterLink>
        <RouterLink to="/services">Services</RouterLink>
        <RouterLink to="/contact">Contact us</RouterLink>
</nav>
</div>
  <RouterView />
</template>

<style scoped>

</style>
