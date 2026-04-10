<script setup lang="ts">
import HeaderBurger from '@/components/HeaderBurger.vue'
import { computed } from 'vue'
</script>

<template>
  <div class="header-description">
    <h1 class="header-title">Даниил Забурунов</h1>
    <p class="text-sm text-[#a1a1aa]">
      Frontend-разработчик. Надёжные интерфейсы для реальных продуктов.
    </p>
  </div>
  <div>
    <div class="header-navigation">
      <a class="header-navigation__item">Обо мне</a>
      <a class="header-navigation__item">Стек</a>
      <a class="header-navigation__item">Проекты</a>
      <a class="header-navigation__item">Контакты</a>
      <a class="header-navigation__item text-white font-semibold">GitHub</a>
      <a class="header-navigation__item text-white font-semibold">Резюме</a>
    </div>
  </div>
  <HeaderBurger />
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
  @apply flex max-lg:hidden flex-row min-[1100px]:gap-8 gap-3 cursor-pointer;
  @apply text-[#a1a1aa] min-[1200px]:text-[14px] text-[12px];
}

.header-navigation__item {
  @apply hover:text-[#18c7ae] hover:shadow-sm shadow-[#18c7ae] rounded-sm p-2;
  @apply transition delay-50 duration-300 ease-in-out;
}
</style>
