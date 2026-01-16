<script setup>
import Connect from "@/app/assets/images/connect.png";
import Create from "@/app/assets/images/create.png";
import Ship from "@/app/assets/images/ship.png";
</script>

<template>
  <section
    class="2xl:pt-23 2xl:pb-30 xl:pt-40 xl:pb-40 lg:pt-10 sm:pt-25 sm:pb-25 pt-20 pb-20 px-4 md:px-16 2xl:px-29 xl:px-20 bg-white"
  >
    <h2
      class="text-[#292462] xl:text-[43px] lg:text-[32px] text-[26px] font-bold text-center 2xl:mb-11 sm:mb-8 mb-5 font-['Satoshi']"
    >
      Control &amp; Power-focused
    </h2>
    <div
      id="scrollContainer"
      class="flex sm:flex-row flex-col items-center justify-between 2xl:w-[1680px] xl:gap-[95px] sm:gap-12 gap-12 snap-x snap-mandatory  [&amp;::-webkit-scrollbar]:hidden [-ms-overflow-style:'none'] [scrollbar-width:'none'] 2xl:pb-3"
    >
      <div class="w-full 2xl:w-[496px] lg:w-[350px] flex-none space-y-3">
        <img :src="Connect" alt="IntelliToggle Control" />
        <div>
          <h3 class="text-[#1A1C3D] font-semibold lg:text-[25px] text-[20px]">
            Connect
          </h3>
          <p class="text-[#5F5F60] 2xl:mt-0 mt-2 lg:text-[18.5px] text-[14px]">
            Install SDK in your Dart project in 2 mins.
          </p>
          <a
            href="#"
            class="inline-flex mt-6 bg-white text-center lg:w-[243px] lg:h-[46px] w-[190px] h-[41px] py-[8px] border-1 border-[#F9A71E] rounded-md text-[#F9A71E] cursor-pointer hover:bg-[#F9A71E] hover:text-[#0F1026] lg:text-[18px] text-[14px] grid place-content-center 2xl:translate-y-1"
          >
            View Documentation
          </a>
        </div>
      </div>
      <div class="w-full 2xl:w-[496px] lg:w-[350px] flex-none space-y-3">
        <img :src="Create" alt="IntelliToggle Control" />
        <div>
          <h3 class="text-[#1A1C3D] font-semibold lg:text-[25px] text-[20px]">
            Create Flags
          </h3>
          <p class="text-[#5F5F60] 2xl:mt-0 mt-2 lg:text-[18.5px] text-[14px]">
            Define features in IntelliToggle dashboard.
          </p>
          <a
            href="#"
            class="inline-flex mt-6 bg-white text-center lg:w-[243px] lg:h-[46px] w-[190px] h-[41px] py-[8px] border-1 border-[#F9A71E] rounded-md text-[#F9A71E] cursor-pointer hover:bg-[#F9A71E] hover:text-[#0F1026] lg:text-[18px] text-[14px] grid place-content-center 2xl:translate-y-1"
          >
            View Documentation
          </a>
        </div>
      </div>
      <div class="w-full 2xl:w-[496px] lg:w-[350px] flex-none space-y-3">
        <img :src="Ship" alt="IntelliToggle Control" />
        <div>
          <h3 class="text-[#1A1C3D] font-semibold lg:text-[25px] text-[20px]">
            Ship &amp; Control
          </h3>
          <p class="text-[#5F5F60] 2xl:mt-0 mt-2 lg:text-[18.5px] text-[14px]">
            Flip switches anytime, see instant results.
          </p>
          <a
            href="#"
            class="inline-flex mt-6 bg-white text-center lg:w-[243px] lg:h-[46px] w-[190px] h-[41px] py-[8px] border-1 border-[#F9A71E] rounded-md text-[#F9A71E] cursor-pointer hover:bg-[#F9A71E] hover:text-[#0F1026] lg:text-[18px] text-[14px] grid place-content-center 2xl:translate-y-1"
          >
            View Documentation
          </a>
        </div>
      </div>
    </div>

    <!-- Dots indicator -->
    <div
      class="relative items-center justify-center hidden w-24 gap-2 mx-auto mt-4 lg:hidden sm:flex"
    >
      <!-- dots -->

      <div class="w-2 h-2 rounded-full bg-[#C5C8E7] relative"></div>
      <div class="w-2 h-2 rounded-full bg-[#C5C8E7] relative"></div>
      <div class="w-2 h-2 rounded-full bg-[#C5C8E7] relative"></div>

      <!-- Highlight bar -->
      <div
        id="highlightBar"
        class="absolute bottom-0 transition-all duration-300 w-10 h-2 rounded-full bg-[#292462]"
        style="left: 0rem"
      ></div>
    </div>
  </section>
</template>
