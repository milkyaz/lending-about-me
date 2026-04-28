<script setup lang="ts">
import { Badge } from '@/components/ui/badge'
import { Button } from '@/components/ui/button'
import { Card, CardContent, CardFooter } from '@/components/ui/card'
import HeroFeatures from './HeroFeatures.vue'
</script>

<template>
  <div class="w-full">
    <Card class="py-4 shadow-none">
      <CardContent
        class="flex max-2xl:flex-col max-2xl:justify-start lg:flex-row flex-wrap justify-between gap-10"
      >
        <div class="flex flex-col max-sm:items-center gap-5">
          <Badge
            class="text-[#14b8a6] text-[11px] [font-family:var(--font-jet)]"
          >
            Лендинг под заявку
          </Badge>
          <h2
            class="text-[28px] max-sm:text-[20px] max-sm:text-center font-semibold text-[#fafafa] leading-[101%]"
          >
            Сайт, который помогает<br />
            получать заявки.
          </h2>
          <p
            class="text-[15px] max-sm:text-center text-[#a7b0be] leading-[148%]"
          >
            Понятно показываю ваши услуги и собираю сайт без лишней сложности.
          </p>
          <div class="flex flex-row max-sm:flex-col flex-wrap gap-2.5">
            <Button class="hero-button">Обсудить сайт</Button>
            <Button class="hero-button">Смотреть кейсы</Button>
          </div>
          <p class="text-[#a1a1aa] [font-family:var(--font-jet)] text-xs">
            Vue · TS · API
          </p>
        </div>
        <div
          class="max-2xl:w-full mt-5 grid sm:grid-cols-2 sm:gap-5 max-sm:grid-cols-1 max-sm:gap-5 max-sm:justify-items-center lg:grid-cols-4 lg:grid-rows-1 lg:gap-5 lg:justify-items-center"
        >
          <HeroFeatures />
        </div>
      </CardContent>
    </Card>
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
  @apply bg-[#131a24] border border-[#2f3a4c] py-7 px-11;
  @apply hover:text-[#0a0a0a] hover:bg-[#14b8a6];
  @apply font-semibold text-[#d7d9df] text-[15px] cursor-pointer;
}
</style>
