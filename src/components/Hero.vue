<script setup lang="ts">
import { Badge } from '@/components/ui/badge'
import { Button } from '@/components/ui/button'
</script>

<template>
  <div class="flex flex-col gap-4">
    <Badge class="hero-badge" variant="outline">Сайты для бизнеса </Badge>
    <h2 class="text-[34px] font-semibold text-[#fafafa] leading-[94%]">
      Сайт, который помогает получать заявки.
    </h2>
    <p class="text-[15px] text-[#a7b0be] leading-[148%]">
      Понятно показываю ваши услуги и собираю сайт без лишней сложности.
    </p>
    <div class="flex flex-col gap-2.5">
      <Button class="hero-button">Обсудить сотрудничество</Button>
      <Button class="hero-button secondary">Смотреть кейсы</Button>
    </div>
    <p class="text-[#a1a1aa] [font-family:var(--font-jet)] text-xs">
      Vue · TS · API
    </p>
  </div>
</template>

<style scoped>
@reference "@/main.css";
.hero-badge {
  @apply w-full justify-start rounded-full border border-[#2f3b4f] px-3 py-2.25;
  @apply bg-linear-to-b from-[#0F131A] to-[#151C25];
  @apply [font-family:var(--font-jet)] text-xs font-medium text-[#b3c0d4];
}

.hero-button {
  @apply w-full bg-[#18c7ae] text-[#05201a] font-bold text-[15px] py-6 px-4.5 rounded-2xl;
}

.secondary {
  @apply bg-[#131a24] border-0 border-[#2f3a4c] font-semibold text-[#d7dee8];
}
</style>
