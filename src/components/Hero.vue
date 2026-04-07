<script setup lang="ts">
import { Badge } from '@/components/ui/badge'
import { Button } from '@/components/ui/button'
</script>

<template>
  <div class="flex flex-col gap-4">
    <Badge class="hero-badge" variant="outline"
      >Frontend Engineer · Vue · TypeScript
    </Badge>
    <h2 class="text-[34px] font-semibold text-[#fafafa] leading-[94%]">
      Frontend, который продаёт и масштабируется.
    </h2>
    <p class="text-[15px] text-[#a7b0be] leading-[148%]">
      Запускаю быстрые интерфейсы с чистым UX, API и адаптивностью.
    </p>
    <div>
      <Button>Получить план работ</Button>
      <Button>Смотреть кейсы</Button>
    </div>
    <p>Vue · TS · API</p>
  </div>
</template>

<style scoped>
@reference "@/main.css";
.hero-badge {
  @apply w-full justify-start rounded-full border border-[#2f3b4f] px-3 py-2.25;
  @apply bg-linear-to-b from-[#0F131A] to-[#151C25];
  @apply [font-family:var(--font-jet)] text-xs font-medium text-[#b3c0d4];
}
</style>
