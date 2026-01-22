<script setup>
import { Analytics } from '@vercel/analytics/nuxt'
</script>

<template>
  <div>
    <NuxtRouteAnnouncer />
    <NuxtPage />
    <Analytics />
  </div>
</template>
