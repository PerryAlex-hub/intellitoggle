<script setup>
import { useRoute } from "vue-router";
import {ref, onMounted, onUnmounted} from "vue"
const route = useRoute();

const atTop = ref(true);

function handleScroll() {
  atTop.value = window.scrollY < 10;
}

onMounted(() => {
  window.addEventListener('scroll', handleScroll);
  handleScroll();
});
onUnmounted(() => {
  window.removeEventListener('scroll', handleScroll);
});
</script>
    
<template>
  <header
    :class="[
      'md:px-16 sm:px-4 2xl:px-29 xl:px-20 w-full fixed top-0 lg:left-0 sm:left-0 z-[5] flex flex-col lg:flex-row sm:flex-row items-start sm:items-center justify-center sm:justify-between lg:gap-0 gap-6 h-screen 2xl:h-[133px] xl:h-[100px] lg:h-[115px] sm:h-[100px] overflow-y-auto lg:overflow-visible -left-[100%] r',
      atTop ? 'bg-transparent' : 'bg-[#42389E]'
    ]"
  >
    <nav
      class="md:px-16 sm:px-4 2xl:px-29 xl:px-20 w-full flex flex-col lg:flex-row sm:flex-row items-start sm:items-center justify-center sm:justify-between lg:gap-0 gap-6 h-[100px] "
    >
      <!-- Logo -->
      <div class="flex shrink-0">
        <NuxtLink to="/" class="text-xl font-bold text-white">
          <img
            class="lg:w-[205.5px] sm:w-[205.5px] w-20"
            src="/images/logo.png"
            alt="Logo"
          />
        </NuxtLink>
      </div>

      <!-- Navigation Links -->
      <div class="hidden text-xl md:flex items-center space-x-8">
        <NuxtLink
          to="/"
          :class="[
            route.path === '/'
              ? 'font-bold text-white pointer-events-none'
              : 'font-normal text-white hover:text-gray-200 transition-colors',
          ]"
        >
          Home
        </NuxtLink>
        <NuxtLink
          to="/about"
          :class="[
            route.path === '/about'
              ? 'font-bold text-white pointer-events-none'
              : 'font-normal text-white hover:text-gray-200 transition-colors',
          ]"
        >
          About
        </NuxtLink>
        <a
          href="#features"
          :class="[
            route.hash === '#features'
              ? 'font-bold text-white pointer-events-none'
              : 'font-normal text-white hover:text-gray-200 transition-colors',
          ]"
        >
          Pricing
        </a>
      </div>

      <!-- CTA Button -->
      <div class="hidden md:flex items-center">
        <a
          href="#"
          class="bg-[#F9A71E] xl:w-[214px] xl:h-[53px] lg:w-[186px] lg:h-[47px] md:h-[41px] w-[210px] h-[50px] rounded-md font-semibold text-[#292462] xl:text-[24px] lg:text-[20px] md:text-[16px] sm:text-[20px] text-[24px] grid place-content-center font-['DM Sans']"
        >
          Start Sandbox
        </a>
      </div>

      <!-- Mobile Menu Button -->
      <div class="md:hidden">
        <button type="button" class="text-white hover:text-gray-900">
          <svg
            class="h-6 w-6"
            fill="none"
            viewBox="0 0 24 24"
            stroke="currentColor"
          >
            <path
              stroke-linecap="round"
              stroke-linejoin="round"
              stroke-width="2"
              d="M4 6h16M4 12h16M4 18h16"
            />
          </svg>
        </button>
      </div>
    </nav>
  </header>
</template>
