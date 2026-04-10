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

.header-burger {
  @apply flex min-lg:hidden flex-row items-start text-4xl;
}

.header-burger__container {
  @apply w-9 h-9 flex flex-row justify-center bg-[#111111] border border-[#262626] rounded-3xl;
}
</style>
