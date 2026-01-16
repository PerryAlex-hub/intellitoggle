<template>
  <div class="min-h-screen flex flex-col">
    <!-- Header -->
    <Header />

    <!-- Main Content -->
    <main class="flex-1 pb-25 ">
      <slot />
    </main>

    <!-- Footer -->
    <Footer />
  </div>
</template>

