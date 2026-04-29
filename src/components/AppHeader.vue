<script setup lang="ts">
import HeaderBurger from '@/components/HeaderBurger.vue'
import { Card, CardContent } from '@/components/ui/card'
import Button from './ui/button/Button.vue'
</script>

<template>
  <Card class="py-4">
    <CardContent
      class="flex flex-row justify-between max-sm:items-start items-center lg:gap-20 gap-5"
    >
      <div class="header-description">
        <h1 class="header-title">Даниил Забурунов</h1>
        <p class="text-sm text-[#a1a1aa]">
          Frontend-разработчик. Надёжные интерфейсы для реальных продуктов.
        </p>
      </div>
      <div>
        <div class="header-navigation">
          <Button class="link header-navigation__item"
            ><a class="">Обо мне</a></Button
          >
          <Button class="link header-navigation__item"
            ><a class="">Стек</a></Button
          >
          <Button class="link header-navigation__item"
            ><a class="">Проекты</a></Button
          >
          <Button class="link header-navigation__item"
            ><a class="">Контакты</a></Button
          >
          <Button class="link header-navigation__item text-white font-semibold"
            ><a class=" ">GitHub</a></Button
          >
          <Button class="link header-navigation__item text-white font-semibold"
            ><a class=" ">Резюме</a></Button
          >
        </div>
      </div>
      <HeaderBurger />
    </CardContent>
  </Card>
</template>
<style scoped>
@reference "@/main.css";

.header-description {
  @apply flex flex-col gap-1.5;
}

.header-title {
  @apply text-xl font-semibold text-white;
}

.header-navigation {
  @apply flex max-lg:hidden flex-row min-[1100px]:gap-8 gap-3;
  @apply text-[#a1a1aa] min-[1200px]:text-[14px] text-[12px];
}

.header-navigation__item {
  @apply hover:text-[#18c7ae] cursor-pointer;
}
</style>
