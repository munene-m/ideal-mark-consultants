<template>
  <div class="">
    <img class="md:h-3/4 h-screen w-full md:top-0 bg-cover"
    src="../assets/images/WhatsApp Image 2022-09-30 at 10.11 1.png" alt="">
  </div>
  
  <div class="flex flex-col md:items-center mx-auto absolute top-40 md:pt-24 md:justify-center md:w-full">
    <img class="relative md:items-center w-28  mx-auto md:w-60 pb-10" src="../assets/images/IdealMark 3.png" alt="">
    <hr>
    <h2 class="text-blue-900 text-center md:text-2xl text-xl font-bold relative flex flex-col md:flex-row">One stop business solutions for
       <p class="text-red-600 font-extrabold pr-2">Marketing</p>and <p class="text-red-600 font-extrabold pl-2">Consultancy</p>needs
    </h2>
    <div class="relative flex flex-row mx-auto gap-6 pt-14">
      <button @click="$router.push('/services')"
        class="bg-red-600 text-white px-2 py-2 rounded-lg border-2 border-red-600 flex-row flex items-center gap-2">Our
        Service
        <ArrowIcon />
      </button>
      <button class="border-white border-2 bg-gray-500 backdrop-filter backdrop-blur-lg bg-opacity-10 text-black px-2 md:px-5 rounded-lg flex-row flex items-center gap-2">Get in touch
        <ArrowIcon />
      </button>
    </div>
  </div>
  <h1 class="text-blue-800 text-4xl font-bold underline italic top-0 bg-gray-200 relative text-center md:pl-8 pt-6">Our customers</h1>
<div class="grid grid-cols-1 md:grid-cols-6 p-8 gap-3 relative top-0 bg-gray-200">
  <div class="w-38">
    <h2 class="font-bold text-black pb-4 flex items-center justify-center md:items-end md:justify-end">UNIVERSAL FORCES INDUSTRIES</h2>
    <p class="italic pb-3 flex items-center justify-center md:items-end md:justify-end">Country - India</p>
    <p class="italic flex items-center justify-center md:items-end md:justify-end">2016 upto date</p>
  </div>
  <div class="w-38">
    <h2 class="font-bold text- pb-4 flex  items-center justify-center md:items-end md:justify-end">PROCIENT ENGINEERING</h2>
    <p class="italic pb-3 flex  items-center justify-center md:items-end md:justify-end ">Country - India</p>
    <p class="italic flex justify-center items-center md:items-end md:justify-end">2017</p>
  </div>
  <div class="w-38">
    <h2 class="font-bold text-black pb-4  items-center justify-center md:items-end md:justify-end flex">INDO AFRICA TRADE EXPO</h2>
    <p class="italic pb-3 flex items-center justify-center md:items-end md:justify-end">Country - India</p>
    <p class="italic flex items-center justify-center md:items-end md:justify-end">2018</p>
  </div>
  <div class="w-38">
    <h2 class="font-bold text-black pb-4 flex items-center justify-center md:items-end md:justify-end">BOSCO INDIAN LTD</h2>
    <p class="italic pb-3 flex  items-center justify-center md:items-end md:justify-end">Country - India</p>
    <p class="italic flex  items-center justify-center md:items-end md:justify-end">2019</p>
  </div>
  <div class="w-38">
    <h2 class="font-bold text-black pb-4 flex items-center justify-center md:items-end md:justify-end">THEMAX HUB ENGINEERING</h2>
    <p class="italic pb-3 flex items-center justify-center md:items-end md:justify-end">Country - India</p>
    <p class="italic flex  items-center justify-center md:items-end md:justify-end">2022</p>
  </div>
  <div class="w-38">
    <h2 class="font-bold text-black flex items-center justify-center md:items-end md:justify-end">SHREENATHJI HYDRAULICS LTD</h2>
    <p class="italic pb-3 flex items-center justify-center md:items-end md:justify-end">Country - India</p>
    <p class="italic flex items-center justify-center md:items-end md:justify-end">2022</p>
  </div>
</div>

</template>
<script setup>
import ArrowIcon from '../assets/icons/ArrowIcon.vue';

</script>