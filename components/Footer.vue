<template>
  <footer class="bg-gray-900 text-white">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 py-12">
      <div class="grid grid-cols-1 md:grid-cols-4 gap-8">
        <!-- Brand -->
        <div class="col-span-1 md:col-span-2">
          <h3 class="text-xl font-bold mb-4">IntelliTogle</h3>
          <p class="text-gray-400 max-w-md">
            Building the future, one toggle at a time. Smart solutions for
            modern problems.
          </p>
        </div>

        <!-- Links -->
        <div>
          <h4 class="font-semibold mb-4">Product</h4>
          <ul class="space-y-2 text-gray-400">
            <li>
              <a href="#" class="hover:text-white transition-colors"
                >Features</a
              >
            </li>
            <li>
              <a href="#" class="hover:text-white transition-colors">Pricing</a>
            </li>
            <li>
              <a href="#" class="hover:text-white transition-colors"
                >Documentation</a
              >
            </li>
          </ul>
        </div>

        <div>
          <h4 class="font-semibold mb-4">Company</h4>
          <ul class="space-y-2 text-gray-400">
            <li>
              <NuxtLink to="/about" class="hover:text-white transition-colors"
                >About</NuxtLink
              >
            </li>
            <li>
              <a href="#" class="hover:text-white transition-colors">Contact</a>
            </li>
            <li>
              <a href="#" class="hover:text-white transition-colors">Privacy</a>
            </li>
          </ul>
        </div>
      </div>

      <div class="border-t border-gray-800 mt-8 pt-8 text-center text-gray-400">
        <p>
          &copy; {{ new Date().getFullYear() }} IntelliTogle. All rights
          reserved.
        </p>
      </div>
    </div>
  </footer>
</template>
