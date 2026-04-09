<script setup lang="ts">
import SectionHeader from '@/components/SectionHeader.vue'
</script>

<template>
  <div class="flex flex-col gap-4">
    <SectionHeader
      title="Что будет на сайте"
      eyebrow="Для бизнеса"
      description="Клиент быстро понимает, чем вы занимаетесь и как с вами связаться."
    />
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
