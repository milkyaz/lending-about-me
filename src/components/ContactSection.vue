<script setup lang="ts">
import { Button } from '@/components/ui/button'
</script>

<template>
  <div class="flex flex-col gap-3">
    <h2 class="text-[#fafafa] text-[26px] font-semibold leading-[102%]">
      Готов помочь с сайтом
    </h2>
    <p class="text-[#a1a1aa] text-[14px] leading-[148%]">
      Под услуги, продажи или рекламу.
    </p>
    <Button>Обсудить сайт</Button>
    <a class="text-[#fafafa] text-[13px] [font-family:var(--font-jet)]"
      >zaburunov.2000@mail.ru</a
    >
    <div
      class="flex flex-row text-[#a1a1aa] text-[13px] leading-[148%] [font-family:var(--font-jet)]"
    >
      <a>Почта</a>
      <span class="mx-2 text-[#262626] text-[13px]"> / </span>
      <a>Telegram</a>
      <span class="mx-2 text-[#262626] text-[13px]"> / </span>
      <a>Резюме</a>
    </div>
  </div>
</template>

<style scoped></style>
