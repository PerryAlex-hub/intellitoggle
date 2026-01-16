<template>
    <section class="px-4 pt-20 pb-20 bg-white 2xl:pt-28 2xl:pb-26 lg:pt-13 lg:pb-20 sm:pt-30 sm:pb-30 md:px-16 2xl:px-29 xl:px-20">
		<h2 class="text-[#292462] xl:text-[43px] lg:text-[32px] text-[26px] font-bold text-center xl:mb-10 lg:mb-7 mb-5 font-['Satoshi'] 2xl:translate-y-1.5">
		Dart-Powered Feature Flag
	</h2>

	<div class="xl:w-[826px] lg:w-[608px] w-full xl:mx-auto xl:text-center lg:text-start">
		<h3 class="text-[#1A1C3D] xl:text-[33px] lg:text-[24px] text-[18px] font-semibold 2xl:translate-y-1.5">
			Not Another Generic Feature Flag Tool
		</h3>
		<p class="text-[#5F5F60] xl:text-[18px] lg:text-[18px] text-[14px] mt-2 xl:mx-10 leading-tight">
			Most tools are built for every language, which means extra layers and slower toggles. IntelliToggle is built in Dart, for Dart — so it's faster, safer, and built for your stack.
		</p>
	</div>
	<div id="scrollContainer" class="2xl:w-[1440px] xl:mx-auto overflow-x-auto [&amp;::-webkit-scrollbar]:hidden [-ms-overflow-style:'none'] [scrollbar-width:'none'] mt-8 mb-3 rounded-bl-lg rounded-br-lg">
		<div class="lg:min-w-full min-w-[1200px] xl:block lg:hidden block">
			<img src="@/app/assets/images/featureFlag.png" alt="Missing Image" class="w-full h-auto">
		</div>

		<div class="min-w-[1600px] h-[318px] lg:inline-block xl:hidden hidden">
			<img src="@/app/assets/images/featureFlag.png" alt="Missing Image" class="object-contain w-full h-full">
		</div>
	</div>
</section>
</template>