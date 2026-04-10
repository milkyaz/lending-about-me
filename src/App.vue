<script setup lang="ts">
import AppHeader from './components/AppHeader.vue'
import Hero from '@/components/Hero.vue'
import About from '@/components/About.vue'
import ProcessSection from '@/components/ProcessSection.vue'
import BusinessTasksSection from '@/components/BusinessTasksSection.vue'
</script>

<template>
  <div class="bg-[#0a0a0a] px-5.5 py-8 flex flex-col gap-13">
    <header class="flex flex-row gap-13"><AppHeader /></header>
    <main class="flex flex-col gap-11">
      <Hero />
      <About />
      <ProcessSection />
      <BusinessTasksSection />
    </main>
  </div>
</template>
