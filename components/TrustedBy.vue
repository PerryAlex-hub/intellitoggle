<script setup>
    import Companies from '@/app/assets/images/companies.png';
</script>
<template>
  <section
    class="px-4 pt-6 pb-10 lg:pt-9 sm:pt-10 sm:pb-10 md:px-16 2xl:px-29 xl:px-20"
  >
    <p
      class="text-center text-[14px] text-[#1A1C3D] xl:text-[25px] lg:text-[16px] sm:text-lg xl:font-semibold sm:font-normal font-medium mt-10 font-['Satoshi'] xl:-translate-y-0 lg:-translate-y-4"
    >
      Trusted by various engineering teams
    </p>
    <div
      class="2xl:max-w-258.75 lg:max-w-[848px] mx-auto flex flex-row items-center justify-start lg:justify-center snap-x snap-mandatory  [&amp;::-webkit-scrollbar]:hidden [-ms-overflow-style:'none'] [scrollbar-width:'none'] 2xl:gap-[100px] lg:gap-[53px] gap-6 xl:mt-8 mt-4"
    >
      <img
        :src="Companies"
        alt="Cloud Provider"
        class="snap-center"
      />
      <!-- <img
        src="/uploads/image/aws.svg"
        alt="Cloud Provider"
        class="snap-center"
      />
      <img
        src="/uploads/image/azure.svg"
        alt="Cloud Provider"
        class="snap-center"
      />
      <img
        src="/uploads/image/digitalocean.svg"
        alt="Cloud Provider"
        class="snap-center"
      />
      <img
        src="/uploads/image/ibm.svg"
        alt="Cloud Provider"
        class="snap-center"
      /> -->
    </div>
  </section>
</template>
