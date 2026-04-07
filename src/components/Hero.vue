<script setup lang="ts">
import { Badge } from '@/components/ui/badge'
</script>

<template>
  <Badge class="hero-badge" variant="default"
    >Frontend Developer / Vue, TypeScript, Vite</Badge
  >
</template>

<style scoped>
@reference "@/main.css";
.hero-badge {
  @apply w-full flex flex-row justify-start p-2 border border-[#262626] bg-[#121212];
  @apply [font-family:var(--font-jet)] text-[#a1a1aa] font-medium text-xs;
}
</style>
