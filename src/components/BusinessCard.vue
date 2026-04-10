<script setup lang="ts">
import { Card, CardContent } from '@/components/ui/card'
import BusinessCardItem from '@/components/BusinessCardItem.vue'
</script>

<template>
  <Card>
    <CardContent class="flex flex-col gap-5">
      <BusinessCardItem
        title="Больше заявок"
        description="Понятная страница под услуги."
        text-btn="Смотреть"
      />
      <BusinessCardItem
        title="Больше продаж"
        description="Простраиваем более понятный путь к покупке."
        text-btn="Смотреть"
      />
      <BusinessCardItem
        title="Сложная услуга"
        description="Объясняем сложное простым языком."
        text-btn="Смотреть"
      />
    </CardContent>
  </Card>
</template>

<style scoped></style>
