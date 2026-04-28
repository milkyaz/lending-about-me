<script setup lang="ts">
import HeroFeaturesItem from './HeroFeaturesItem.vue'

const heroFeatures = [
  {
    id: 1,
    title: 'Понятная структура',
    description:
      'Сайт помогает быстро понять, что вы предлагаете и зачем оставлять заявку.',
    icon: 'ph:network-light',
  },
  {
    id: 2,
    title: 'Сильный первый экран',
    description:
      'Заголовок, акценты и кнопки сразу ведут пользователя к действию.',
    icon: 'ph:target-light',
  },
  {
    id: 3,
    title: 'Адаптивная вёрстка',
    description:
      'Интерфейс корректно работает на телефоне, планшете и десктопе.',
    icon: 'ph:monitor-light',
  },
  {
    id: 4,
    title: 'Готовность к развитию',
    description:
      'Можно подключать формы, API, новые секции и развивать сайт дальше.',
    icon: 'ph:code-light',
  },
]
</script>
<template>
  <HeroFeaturesItem
    v-for="item in heroFeatures"
    :key="item.id"
    :icon-name="item.icon"
    :title="item.title"
    :text="item.description"
  />
</template>

<style scoped>
@reference "@/main.css";
</style>
