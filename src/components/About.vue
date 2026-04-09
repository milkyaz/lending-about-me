<script setup lang="ts"></script>

<template>
  <div class="flex flex-col gap-4">
    <p class="text-[#14b8a6] text-[11px] [font-family:var(--font-jet)]">
      Для бизнеса
    </p>
    <h2 class="text-[#fafafa] text-[28px] font-semibold leading-[106%]">
      Что будет на сайте
    </h2>
    <p class="text-[#a1a1aa] text-[14px] leading-[148%]">
      Клиент быстро понимает, чем вы занимаетесь и как с вами связаться.
    </p>
    <div class="flex flex-col gap-4">
      <div class="about-card-item">
        <h4 class="about-card__title">Понятно</h4>
        <p class="about-card__text">Сразу видно, что вы предлагаете.</p>
      </div>
      <div class="about-card-item">
        <h4 class="about-card__title">Связь</h4>
        <p class="about-card__text">Форма, Telegram и почта на виду.</p>
      </div>
      <div class="about-card-item">
        <h4 class="about-card__title">Правки</h4>
        <p class="about-card__text">Тексты и услуги легко обновлять.</p>
      </div>
    </div>
  </div>
</template>

<style scoped>
@reference "@/main.css";

.about-card-item {
  @apply p-4 border border-[#262626] rounded-[18px] bg-[#121212];
}

.about-card__title {
  @apply text-[#fafafa] text-[17px] font-semibold;
}

.about-card__text {
  @apply text-[#a1a1aa] text-[14px] leading-[148%];
}
</style>
