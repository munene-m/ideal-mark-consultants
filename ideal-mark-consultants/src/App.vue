

<template>
 <div class="md:flex md:flex-row md:justify-between hidden md:pl-10 md:w-11/12 md:bg-gray-600 md:backdrop-filter md:backdrop-blur-lg md:bg-opacity-30 md:z-10 md:absolute md:top-0">
    <div class="flex md:flex-row md:gap-5 md:text-black md:items-end md:pb-2">
      <WhatsappIcon />
      <TwitterIcon />
      <InstagramIcon />
      <FacebookIcon />
    </div>
    <div class="flex md:flex-row md:justify-center md:text-black md:items-end gap-4 mr-4">
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
  <div class="flex top-10 md:w-full md:absolute md:top-12 md:z-20 p-0 m-0 box-border">
    <nav
      class=" p-4 md:flex md:justify-between md:items-end md:space-x-10 text-black border-b bg-gray-800 backdrop-filter backdrop-blur-lg bg-opacity-20 relative border-gray-200  w-full border-r-0 border-l-0 pr-10">
      <div class="flex items-start justify-between">
        <RouterLink to="/" ><img class="w-24" src="./assets/images/IdealMark 2.png" alt=""></RouterLink>
        <!--Mobilemenu button-->
        <div @click="toggleNav" class="flex md:hidden">
          <button type="button" class="text-gray-800 hover:text-red-400 focus:outline-none focus:text-gray-900">
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
  <RouterView />
  <About/>
</template>

<style scoped>
</style>

<script setup>
import { ref } from 'vue';
import { RouterLink, RouterView } from 'vue-router';
import WhatsappIcon from './assets/icons/WhatsappIcon.vue';
import FacebookIcon from './assets/icons/FacebookIcon.vue';
import TwitterIcon from './assets/icons/TwitterIcon.vue';
import InstagramIcon from './assets/icons/InstagramIcon.vue';
import MenuIcon from './assets/icons/MenuIcon.vue'
import About from './views/About.vue';
import Services from './views/Services.vue';
let showMenu = ref(false)
function toggleNav() {
  return (showMenu.value = !showMenu.value);
}
</script>
