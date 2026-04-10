<script setup lang="ts">
import SectionHeader from '@/components/SectionHeader.vue'
import BusinessCard from '@/components/BusinessCard.vue'
</script>

<template>
  <div class="flex flex-col gap-4">
    <SectionHeader
      title="Какие задачи может решать сайт"
      eyebrow="Где сайт помогает"
      description="Вот несколько задач бизнеса."
    />
  </div>
  <BusinessCard />
</template>

<style scoped>
@reference "@/main.css";
</style>
