<template>
  <div class="absolute">
    <img class="h-full w-full  object-cover top-0 bg-cover"
    src="../assets/images/WhatsApp Image 2022-09-30 at 10.11 1.png" alt="">
  </div>
  
  <div class="md:flex md:flex-row md:justify-between md:items-end md:z-10 md:relative md:top-8 md:text-white md:ml-4">
    <div class="flex md:flex-row md:gap-4 md:place-items-end">
      <WhatsappIcon />
      <TwitterIcon />
      <InstagramIcon />
      <FacebookIcon />
    </div>
    <div class="flex md:flex-row md:justify-center md:items-center gap-4 mr-4">
      <ul>
        <li>Phone number</li>
        <li>+254 722928160</li>
      </ul>
      <ul>
        <li>Free Consultancy</li>
        <li>ceo@idealmarkconsultants</li>
      </ul>
    </div>
  </div>
  <div class="flex top-10 relative z-10  p-0 m-0 box-border">
    <nav
      class=" p-4 md:flex md:justify-between md:items-end md:space-x-10 text-white border-white border-2 w-full border-r-0 border-l-0 pr-10">
      <div class="flex items-start justify-between">
        <RouterLink to="/" class="text-xl flex md:items-start md:justify-start gap-1 font-bold text-gray-100 md:text-2xl hover:text-green-400">
          <img src="./assets/images/IdealMark 2.png" alt="">
        </RouterLink>
        <!--Mobilemenu button-->
        <div @click="toggleNav" class="flex md:hidden">
          <button type="button" class="text-gray-100 hover:text-green-400 focus:outline-none focus:text-gray-400">
            <MenuIcon />
          </button>
        </div>
      </div>
      <ul :class="showMenu ? 'flex' : 'hidden'" class="flex-col mt-8 space-y-4 md:flex md:space-y-0 md:flex-row md:items-center md:space-x-10 md:mt-0">
        <li><RouterLink to="/">Home</RouterLink></li>
        <li><RouterLink to="/about">About Us</RouterLink></li>
        <li><RouterLink to="/services">Services</RouterLink></li>
        <li><RouterLink to="/contact">Contact us</RouterLink></li>
      </ul>
    </nav>

  </div>
  <div class="flex flex-col md:items-center md:pt-24 md:justify-center md:w-full">
    <img class="relative md:items-center w-60 pb-10" src="../assets/images/IdealMark 3.png" alt="">
    <hr>
    <h2 class="text-blue-900/100 text-xl font-bold relative flex flex-row">One stop business solutions for <p
        class="text-red-600 font-extrabold">Marketing</p> and <p class="text-red-600 font-extrabold">Consultancy</p>
      needs</h2>
    <div class="relative flex flex-row gap-6 pt-14">
      <button
        class="bg-red-600 text-white px-5 py-2 rounded-lg border-2 border-red-600 flex-row flex items-center gap-2">Our
        Service
        <ArrowIcon />
      </button>
      <button class="border-white border-2 text-white px-5 rounded-lg flex-row flex items-center gap-2">Get in touch
        <ArrowIcon />
      </button>
    </div>
  </div>
  <h1 class="text-blue-800 text-4xl font-bold underline italic top-56 bg-white text-center md:pl-8 pt-6  relative">Our customers</h1>
<div class="grid grid-cols-1 md:grid-cols-6 p-8 gap-3 top-56 bg-white relative">
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
<RouterView/>
</template>
<script setup>
import { ref } from 'vue';
import { RouterLink, RouterView } from 'vue-router';
import ArrowIcon from '../assets/icons/ArrowIcon.vue';
import WhatsappIcon from '../assets/icons/WhatsappIcon.vue';
import FacebookIcon from '../assets/icons/FacebookIcon.vue';
import TwitterIcon from '../assets/icons/TwitterIcon.vue';
import InstagramIcon from '../assets/icons/InstagramIcon.vue';
let showMenu = ref(false)
function toggleNav() {
  return (showMenu.value = !showMenu.value);
}
</script>