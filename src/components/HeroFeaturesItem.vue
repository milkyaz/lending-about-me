<script setup lang="ts">
import { Card, CardContent } from '@/components/ui/card'
import { Icon } from '@iconify/vue'

type Props = {
  iconName: string
  title: string
  text: string
}

const { iconName, title, text } = defineProps<Props>()
</script>

<template>
  <Card class="w-50 h-50 bg-[#16181A] py-0 justify-center">
    <CardContent class="flex flex-col items-center gap-3 text-white">
      <Icon
        :icon="iconName"
        class="border border-[#575757] bg-[#282829] rounded-2xl p-2"
        width="60"
      />
      <h3 class="text-xl text-center font-semibold">{{ title }}</h3>
    </CardContent>
  </Card>
</template>

<style scoped>
@reference "@/main.css";
</style>
