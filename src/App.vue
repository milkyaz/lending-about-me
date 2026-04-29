<script setup lang="ts">
import AppHeader from './components/AppHeader.vue'
import Hero from '@/components/Hero.vue'
import About from '@/components/About.vue'
import ProcessSection from '@/components/ProcessSection.vue'
import BusinessTasksSection from '@/components/BusinessTasksSection.vue'
import ContactSection from '@/components/ContactSection.vue'
</script>

<template>
  <div
    class="bg-[#0a0a0a] max-lg:px-5.5 px-10 py-8 flex flex-col gap-13 2xl:px-50"
  >
    <header><AppHeader /></header>
    <main class="flex flex-col gap-11 items-center">
      <Hero />
      <About />
      <ProcessSection />
      <BusinessTasksSection />
    </main>
    <footer class="flex flex-col gap-11 items-center">
      <ContactSection />
    </footer>
  </div>
</template>
