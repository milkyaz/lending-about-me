<script setup lang="ts">
import AppHeader from './components/AppHeader.vue'
import Hero from '@/components/Hero.vue'
</script>

<template>
  <div class="bg-[#0a0a0a] px-5.5 py-8 flex flex-col gap-13">
    <header class="flex flex-row gap-13"><AppHeader /></header>
    <main><Hero /></main>
  </div>
</template>
