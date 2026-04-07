<script setup lang="ts">
import { Badge } from '@/components/ui/badge'
</script>

<template>
  <Badge class="hero-badge" variant="outline"
    >Frontend Engineer · Vue · TypeScript</Badge
  >
</template>

<style scoped>
@reference "@/main.css";
.hero-badge {
  @apply w-full justify-start rounded-full border border-[#2f3b4f] px-3 py-2.25;
  @apply bg-linear-to-b from-[#0F131A] to-[#151C25];
  @apply [font-family:var(--font-jet)] text-xs font-medium text-[#b3c0d4];
}
</style>
