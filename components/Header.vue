<script setup>
import { useRoute } from "vue-router";
import { ref, onMounted, onUnmounted } from "vue";
const route = useRoute();

const atTop = ref(true);
const mobileOpen = ref(false);

function handleScroll() {
  atTop.value = window.scrollY < 10;
}

function toggleMobile() {
  mobileOpen.value = !mobileOpen.value;
}

onMounted(() => {
  window.addEventListener("scroll", handleScroll);
  handleScroll();
});
onUnmounted(() => {
  window.removeEventListener("scroll", handleScroll);
});
</script>

<template>
  <header
    :class="[
      'w-full fixed top-0 left-0 z-50 transition-all h-20 xl:h-[133px]',
      atTop ? 'bg-transparent' : 'bg-[#42389E] ',
    ]"
  >
    <nav class="w-full flex items-center justify-between px-4  md:px-29 h-full">
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
          class="bg-[#F9A71E] xl:w-[214px] xl:h-[53px] lg:w-[186px] lg:h-[47px] md:h-[41px] w-[210px] h-[50px] rounded-md font-semibold text-[#292462] xl:text-[24px] lg:text-[20px] md:text-[16px] sm:text-[20px]  text-[24px] grid place-content-center font-['DM Sans']"
        >
          Start Sandbox
        </a>
      </div>

      <!-- Mobile Menu Button -->
      <div class="md:hidden">
        <button
          type="button"
          class="text-white hover:text-gray-900"
          @click="toggleMobile"
        >
          <img src="@/app/assets/images/mobile-menu.png" />
        </button>
      </div>
    </nav>

    <!-- Mobile dropdown -->
    <div
      v-if="mobileOpen"
      class="md:hidden w-full fixed top-20 left-0 z-40 bg-[#42389E] py-4"
    >
      <div class="flex flex-col items-center space-y-3">
        <NuxtLink to="/" class="text-white text-lg" @click="mobileOpen = false"
          >Home</NuxtLink
        >
        <NuxtLink
          to="/about"
          class="text-white text-lg"
          @click="mobileOpen = false"
          >About</NuxtLink
        >
        <a
          href="#features"
          class="text-white text-lg"
          @click="mobileOpen = false"
          >Pricing</a
        >
        <a
          href="#"
          class="bg-[#F9A71E] w-35 h-[50px] rounded-md font-semibold text-[#292462] text-lg grid place-content-center font-['DM Sans']"
        >
          Start Sandbox
        </a>
      </div>
    </div>
  </header>
</template>
