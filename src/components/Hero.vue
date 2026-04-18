<script setup lang="ts">
import { Badge } from '@/components/ui/badge'
import { Button } from '@/components/ui/button'
import { Card, CardContent, CardFooter } from '@/components/ui/card'
</script>

<template>
  <Card
    class="py-4 flex flex-row max-[1100px]:bg-transparent max-[1100px]:border-0 max-[1100px]:shadow-none max-[1100px]:rounded-none"
  >
    <CardContent class="flex flex-col gap-5">
      <Badge class="text-[#14b8a6] text-[11px] [font-family:var(--font-jet)]">
        Лендинг под заявку
      </Badge>
      <h2 class="text-[58px] font-semibold text-[#fafafa] leading-[101%]">
        Сайт, который помогает получать заявки.
      </h2>
      <p class="text-[15px] text-[#a7b0be] leading-[148%]">
        Понятно показываю ваши услуги и собираю сайт без лишней сложности.
      </p>
      <div class="flex flex-row gap-2.5">
        <Button class="hero-button">Обсудить сайт</Button>
        <Button class="hero-button secondary">Смотреть кейсы</Button>
      </div>
      <p class="text-[#a1a1aa] [font-family:var(--font-jet)] text-xs">
        Vue · TS · API
      </p>
    </CardContent>
    <CardFooter class="flex flex-col justify-center items-center w-100">
      <div
        class="w-90 h-60 bg-cover bg-[url(/src/assets/images/desktopPanelsExport.png)]"
      ></div>
      <!--      <img class="bg-cover" src="" alt="hero-png" />-->
      <hr class="border border-[#ffffff10] w-85" />
    </CardFooter>
  </Card>
</template>

<style scoped>
@reference "@/main.css";
.hero-badge {
  @apply w-full justify-start rounded-full border border-[#2f3b4f] px-3 py-2.25;
  @apply bg-linear-to-b from-[#0F131A] to-[#151C25];
  @apply [font-family:var(--font-jet)] text-xs font-medium text-[#b3c0d4];
}

.hero-button {
  @apply bg-[#131a24] border border-[#2f3a4c] py-7 px-11;
  @apply hover:text-[#0a0a0a] hover:bg-[#14b8a6];
  @apply font-semibold text-[#d7d9df] text-[15px] cursor-pointer;
}
</style>
