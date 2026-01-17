<template>
  <footer
    class="2xl:px-29 xl:px-20 xl:pt-25 md:px-16 px-4 lg:pt-20 pt-16 lg:pb-16 pb-8 bg-[#ECEBF5]"
  >
    <div
      class="grid grid-cols-9 2xl:gap-5 lg:gap-0 sm:gap-3 gap-6 w-full 2xl:translate-y-[14px]"
    >
      <div class="col-span-9 lg:col-span-3 sm:col-span-3">
        <img
          src="/images/blue-logo.png"
          alt="Intellitoggle Logo"
          class="xl:w-[170.5px] mb-2"
        />

        <p
          class="text-[#4A4B4D] py-4 xl:text-[18.5px] xl:w-[348px] xl:w-[379px] lg:w-[300px] leading-tight 2xl:-translate-y-[8px] 2xl:translate-x-[2px]"
        >
          IntelliToggle is built by AORTEM, a company focused on powering
          scalable, multi-platform developer tools
        </p>

        <div class="flex flex-row mb-6 gap-x-3">
          <a
            href="https://github.com/aortem"
            class="inline-block 2xl:translate-x-[4px] 2xl:-translate-y-[6px]"
          >
            <div
              class="rounded-full bg-[#4B4B4B] flex justify-center items-center"
            >
              <img src="/images/github-logo.png" alt="Social Media Icon" />
            </div>
          </a>
        </div>
      </div>

      <div
        class="2xl:col-span-2 xl:col-span-2 lg:col-span-3 sm:col-span-3 col-span-5 xl:text-[18px] order-3 lg:order-3 xl:order-2 2xl:pl-10"
      >
        <h3 class="mb-4 text-[#5F5F60]">Resources</h3>
        <div class="space-y-3 flex flex-col text-[#323338] font-semibold">
          <a
            href="https://www.intellitoggle.com/why-us"
            class="inline-block cursor-pointer"
            >Why IntelliToggle is Different</a
          >
          <a
            href="https://aortem-prod.web.app/login"
            class="inline-block cursor-pointer"
            >Customer Support</a
          >
          <a
            href="https://www.intellitoggle.com/terms/terms-of-service"
            class="inline-block cursor-pointer"
            >Terms &amp; Conditions</a
          >
          <a
            href="https://www.intellitoggle.com/terms/privacy-policy"
            class="inline-block cursor-pointer"
            >Privacy Policy</a
          >
          <a
            href="https://www.intellitoggle.com/terms/refund-policy"
            class="inline-block cursor-pointer"
            >Refund Policy</a
          >
        </div>
      </div>

      <div
        class="2xl:col-span-2 xl:col-span-2 lg:col-span-3 sm:col-span-3 col-span-4 xl:text-[18px] order-2 lg:order-2 2xl:pl-8 lg:pl-8"
      >
        <h3 class="mb-4 text-[#5F5F60]">Company</h3>
        <div class="space-y-3 flex flex-col text-[#323338] font-semibold">
          <a
            href="https://www.intellitoggle.com/pricing"
            class="inline-block cursor-pointer"
            >Pricing</a
          >
          <a
            href="https://docs.intellitoggle.com"
            class="inline-block cursor-pointer"
            >Documentation</a
          >
          <a
            href="https://www.intellitoggle.com/about"
            class="inline-block cursor-pointer"
            >About Us</a
          >
          <a
            href="https://www.intellitoggle.com/contact-us"
            class="inline-block cursor-pointer"
            >Contact Us</a
          >
        </div>
      </div>

      <div
        class="2xl:col-span-2 xl:col-span-2 lg:col-span-8 sm:col-span-3 col-span-9 xl:text-[18px] 2xl:place-content-start xl:place-content-center w-full lg:place-content-center sm:place-content-end 2xl:mr-6 xl:mr-0 lg:mt-6 lg:mr-6 mt-16 order-4 lg:order-4 2xl:translate-y-8"
      >
        <div class="flex flex-col items-end justify-end 2xl:mt-10 lg:mt-5">
          <form
            id="subscribeForm"
            class="flex flex-row items-center justify-start 2xl:w-[321px] lg:w-[321px] lg:h-[45.8px] h-[45.8px] w-full xl:h-[49px] relative"
          >
            <h2 class="absolute -top-13 text-[#323338] font-semibold">
              Subscribe to Newsletter
            </h2>
            <input
              type="email"
              id="userEmail"
              class="xl:px-4 px-3 bg-white outline-none border-none w-full h-full text-sm rounded-l-[6.67px] lg:placeholder:text-[11.67px]"
              placeholder="Enter your email address"
            />
            <button
              type="submit"
              class="lg:text-[13.33px] text-sm lg:w-[115.8px] lg:h-[49px] w-[115.8px] h-full lg:bg-[#F9A71E] lg:from-[#F9A71E] lg:to-[#F9A71E] lg:text-[#292462] bg-gradient-to-t from-[#0F1026] to-[#42389E] text-white px-2 shrink-0 outline-none rounded-r-md cursor-pointer font-semibold"
            >
              <span class="hidden xl:block">Subscribe</span>
              <span class="block xl:hidden">Join</span>
            </button>
          </form>
          <p
            id="errorMessage"
            class="pt-2 text-base font-semibold text-red-500"
          ></p>
        </div>
      </div>
    </div>
    <!-- Copyright -->
    <div class="pt-6 mt-8">
      <p class="text-center text-[#4A4B4D] text-[16px]">
        © 2026 All rights reserved.
      </p>
    </div>
  </footer>
</template>
