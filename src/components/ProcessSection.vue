<script setup lang="ts">
import { Check, Circle, Dot } from 'lucide-vue-next'
import { Button } from '@/components/ui/button'
import {
  Stepper,
  StepperDescription,
  StepperItem,
  StepperSeparator,
  StepperTitle,
  StepperTrigger,
} from '@/components/ui/stepper'

const steps = [
  {
    step: 1,
    title: 'Задача',
    description: 'Чем занимаетесь/Кто клиент/Что важно',
  },
  {
    step: 2,
    title: 'Макет',
    description: 'Блоки/Тексты/Связь',
  },
  {
    step: 3,
    title: 'Сайт',
    description: 'Tailwind/Vue/Адаптив',
  },
  {
    step: 4,
    title: 'Запуск',
    description: 'Проверка/Публикация/Правки',
  },
]

const activeStep = 3
</script>

<template>
  <div class="flex flex-col gap-4">
    <p class="text-[#14b8a6] text-[11px] [font-family:var(--font-jet)]">
      Процесс
    </p>
    <h2 class="text-[#fafafa] text-[28px] font-semibold leading-[106%]">
      Как делаю сайт
    </h2>
    <p class="text-[#a1a1aa] text-[14px] leading-[148%]">
      Понять задачу, собрать, запустить.
    </p>
    <Stepper
      :default-value="activeStep"
      orientation="vertical"
      class="mx-auto flex w-full max-w-md flex-col justify-start gap-10"
    >
      <StepperItem
        v-for="step in steps"
        :key="step.step"
        v-slot="{ state }"
        class="relative flex w-full items-start gap-6"
        :step="step.step"
      >
        <StepperSeparator
          v-if="step.step !== steps[steps.length - 1]?.step"
          class="absolute left-[18px] top-[38px] block h-[105%] w-0.5 shrink-0 rounded-full bg-muted group-data-[state=completed]:bg-[#18c7ae]"
        />
        <StepperTrigger as-child>
          <Button
            :variant="
              state === 'completed' || state === 'active'
                ? 'default'
                : 'outline'
            "
            size="icon"
            class="z-10 rounded-full shrink-0"
            :class="[state === 'active' && 'ring-2 ring-[#05201a]']"
          >
            <Check v-if="state === 'completed'" class="size-5" />
            <Circle v-if="state === 'active'" />
            <Dot v-if="state === 'inactive'" />
          </Button>
        </StepperTrigger>
        <div class="flex flex-col gap-1">
          <StepperTitle
            :class="[state === 'active' && 'text-primary']"
            class="text-[#fafafa] text-[17px] font-semibold transition lg:text-base"
          >
            {{ step.title }}
          </StepperTitle>
          <StepperDescription
            :class="[state === 'active' && 'text-primary']"
            class="text-xs text-muted-foreground transition lg:text-sm"
          >
            {{ step.description }}
          </StepperDescription>
        </div>
      </StepperItem>
    </Stepper>
  </div>
</template>

<style scoped>
@reference "@/main.css";
</style>
