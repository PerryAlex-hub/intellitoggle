<script setup>
import WhatIs from "@/app/assets/images/WhatIs.png";
</script>

<template>
  <section
    class="px-4 pt-20 pb-20 2xl:pt-49 xl:pt-36 lg:pt-22 sm:pt-4 sm:pb-36 md:px-16 2xl:px-29 xl:px-20"
  >
    <h2
      class="text-[#292462] xl:text-[42px] lg:text-[32px] sm:text-[32px] text-3xl font-bold text-center sm:mb-14 mb-5 font-['Satoshi'] 2xl:translate-y-2"
    >
      What is IntelliToggle
    </h2>
    <div class="flex flex-col items-center justify-between gap-6 lg:flex-row">
      <div class="2xl:w-[623px] xl:w-full lg:w-[469px] 2xl:px-[5px] w-full">
        <h3
          class="xl:text-[32px] lg:text-[24px] text-[26px] text-[#323338] font-semibold leading-tight 2xl:mt-2 xl:-translate-y-0 lg:-translate-y-4"
        >
          Your AI Dart App's Control Panel For Feature Releases
        </h3>
        <p
          class="text-[#5F5F60] mt-3 mb-1 xl:text-[18px] lg:text-[14px] sm:text-[15px] text-[14px] leading-tight xl:-translate-y-0 lg:-translate-y-4"
        >
          IntelliToggle is a “Dart-Powered” feature flag that lets you turn
          features on/off instantly in your application without redeploying
          code. It allows you control roll-outs, run experiments, and fix bugs
          faster.
        </p>
        <h4
          class="xl:text-[24px] lg:text-[22px] text-[18px] text-[#323338] font-semibold 2xl:translate-y-0 xl:-translate-y-0 lg:-translate-y-4"
        >
          Benefits
        </h4>
        <ul
          class="list-disc list-inside text-[#5F5F60] xl:text-[18px] text-[14px] leading-tight 2xl:translate-y-2 xl:-translate-y-0 lg:-translate-y-3"
        >
          <li class="ml-[10px]">Toggle new features without app update</li>
          <li class="ml-[10px]">Roll out to specific users or regions</li>
          <li class="ml-[10px]">Instantly rollback when needed</li>
        </ul>
      </div>
      <div
        class="2xl:w-[835px] xl:w-full lg:w-[383px] w-full lg:rounded-[12px] rounded-[8px] 2xl:p-[51px] lg:px-[40px] lg:py-[30px] p-[20px] bg-gradient-to-t from-[#0F1026] to-[#42389E] lg:mt-0 mt-3"
      >
        <img :src="WhatIs" alt="Logo" class="w-full" />
      </div>
    </div>
  </section>
</template>
