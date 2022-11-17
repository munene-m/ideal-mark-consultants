<script setup>
import { RouterLink, RouterView } from 'vue-router'
import { ref } from 'vue';
import MenuIcon from './components/MenuIcon.vue'
import WhatsappIcon from './assets/icons/WhatsappIcon.vue'
import InstagramIcon from './assets/icons/InstagramIcon.vue'
import TwitterIcon from './assets/icons/TwitterIcon.vue'
import FacebookIcon from './assets/icons/FacebookIcon.vue'
let showMenu = ref(false)
function toggleNav() {
  return (showMenu.value = !showMenu.value);
}
</script>

<template>
  <img class="h-full w-full m-0 p-0 object-cover absolute bg-cover"
    src="./assets/images/WhatsApp Image 2022-09-30 at 10.11 1.png" alt="">
  <div class="flex flex-col text-black md:flex-row md:justify-between items-end relative top-16 md:text-white ml-4">
    <div class="flex md:flex-row gap-4 md:place-items-end justify-center text-center">
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
  <div class="flex py-20 bg-transparent p-0 m-0 box-border">
    <nav
      class="relative p-4 md:flex md:justify-between md:items-end md:space-x-10 text-white border-white border-2 w-full border-r-0 border-l-0 pr-10">

      <div class="flex items-start justify-between">
        <RouterLink to="/"
          class="text-xl flex md:items-start md:justify-start gap-1 font-bold text-gray-100 md:text-2xl hover:text-green-400">
          <img src="./assets/images/IdealMark 2.png" alt="">
        </RouterLink>
        <!--Mobilemenu button-->
        <div @click="toggleNav" class="flex md:hidden">
          <button type="button" class="text-gray-100 hover:text-green-400 focus:outline-none focus:text-gray-400">
            <MenuIcon />
          </button>
        </div>
      </div>
      <ul :class="showMenu ? 'flex' : 'hidden'"
        class="flex-col mt-8 space-y-4 md:flex md:space-y-0 md:flex-row md:items-center md:space-x-10 md:mt-0">
        <li>
          <RouterLink to="/">Home</RouterLink>
        </li>
        <li>
          <RouterLink to="/about">About Us</RouterLink>
        </li>
        <li>
          <RouterLink to="/services">Services</RouterLink>
        </li>
        <li>
          <RouterLink to="/contact">Contact us</RouterLink>
        </li>
      </ul>
    </nav>

  </div>
  <RouterView />
</template>

<style scoped>

</style>
