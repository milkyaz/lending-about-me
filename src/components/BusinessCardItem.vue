<script setup lang="ts">
import {
  Item,
  ItemActions,
  ItemContent,
  ItemDescription,
  ItemTitle,
} from '@/components/ui/item'
import { Button } from '@/components/ui/button'
type Props = {
  title: string
  description: string
  textBtn: string
}
const {} = defineProps<Props>()
</script>

<template>
  <Item class="task-item">
    <ItemContent>
      <ItemTitle class="text-[#fafafa]">{{ title }}</ItemTitle>
      <ItemDescription>{{ description }}</ItemDescription>
    </ItemContent>
    <ItemActions>
      <Button variant="outline" size="sm">{{ textBtn }}</Button>
    </ItemActions>
  </Item>
</template>

<style scoped>
@reference "@/main.css";

.task-item {
  @apply border border-[#18c7ae] bg-[#131a24];
}
</style>
