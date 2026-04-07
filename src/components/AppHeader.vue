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
  <div class="flex flex-row gap-13">
    <div class="flex flex-col border-2 border-amber-800 gap-1.5">
      <h1 class="text-xl font-semibold text-white">Даниил Забурунов</h1>
      <p class="text-sm text-[#a1a1aa]">
        Frontend-разработчик. Спокойные, надёжные интерфейсы для реальных
        продуктов.
      </p>
    </div>
    <div
      class="flex flex-row items-start text-4xl text-[orange] border-2 border-purple-900"
    >
      <div
        class="w-9 h-9 flex flex-row justify-center bg-[#111111] border border-[#262626] rounded-3xl"
      >
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
  </div>
</template>
