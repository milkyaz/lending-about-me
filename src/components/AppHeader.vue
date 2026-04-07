<script setup lang="ts">
import {
  Sheet,
  SheetContent,
  SheetDescription,
  SheetHeader,
  SheetTrigger,
} from '@/components/ui/sheet'
</script>

<template>
  <div class="header-description">
    <h1 class="header-title">Даниил Забурунов</h1>
    <p class="text-sm text-[#a1a1aa]">
      Frontend-разработчик. Надёжные интерфейсы для реальных продуктов.
    </p>
  </div>
  <div class="header-burger">
    <div class="header-burger__container">
      <Sheet>
        <SheetTrigger
          ><img
            class="w-3.5"
            src="/src/assets/images/menuIcon.webp"
            alt="menu-icon"
          />
        </SheetTrigger>
        <SheetContent class="border-l-2 border-[#101010] bg-black">
          <SheetHeader>
            <SheetDescription>
              <div class="flex flex-col text-[#a1a1aa]">
                <a>Обо мне</a>
                <a>Стек</a>
                <a>Проекты</a>
                <a>Контакты</a>
                <a class="text-white font-semibold">GitHub</a>
                <a class="text-white font-semibold">Резюме</a>
              </div>
            </SheetDescription>
          </SheetHeader>
        </SheetContent>
      </Sheet>
    </div>
  </div>
</template>
<style scoped>
@reference "@/main.css";

.header-description {
  @apply flex flex-col border-2 border-amber-800 gap-1.5;
}

.header-title {
  @apply text-xl font-semibold text-white;
}

.header-burger {
  @apply flex flex-row items-start text-4xl text-[orange] border-2 border-purple-900;
}

.header-burger__container {
  @apply w-9 h-9 flex flex-row justify-center bg-[#111111] border border-[#262626] rounded-3xl;
}
</style>
