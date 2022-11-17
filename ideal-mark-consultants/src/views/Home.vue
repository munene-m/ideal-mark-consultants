<template>
  <div class="flex flex-col md:items-center md:justify-center md:w-full">
    <img class="relative md:items-center w-60 pb-10" src="../assets/images/IdealMark 3.png" alt="">
    <hr>
    <h2 class="text-blue-900/100 text-xl font-bold relative flex flex-row">One stop business solutions for <p class="text-red-600 font-extrabold">Marketing</p> and <p class="text-red-600 font-extrabold">Consultancy</p> needs</h2>
    <div class="relative flex flex-row gap-6 pt-14">
        <button class="bg-red-600 text-white px-5 py-2 rounded-lg border-2 border-red-600 flex-row flex items-center gap-2">Our Service<ArrowIcon/></button>
        <button class="border-white border-2 text-white px-5 rounded-lg flex-row flex items-center gap-2">Get in touch<ArrowIcon/></button>
    </div>
  </div>
</template>
<script setup>
import ArrowIcon from '../assets/icons/ArrowIcon.vue';
</script>