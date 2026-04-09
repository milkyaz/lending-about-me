<script setup lang="ts">
type Props = {
  eyebrow: string
  title: string
  description: string
}

const { eyebrow, title, description } = defineProps<Props>()
</script>

<template>
  <p class="text-[#14b8a6] text-[11px] [font-family:var(--font-jet)]">
    {{ eyebrow }}
  </p>
  <h2 class="text-[#fafafa] text-[28px] font-semibold leading-[106%]">
    {{ title }}
  </h2>
  <p class="text-[#a1a1aa] text-[14px] leading-[148%]">
    {{ description }}
  </p>
</template>

<style scoped></style>
