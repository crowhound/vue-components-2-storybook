<script setup lang="ts">
defineProps<{
  hours: number
  minutes: number
  seconds: number
}>()
</script>

<template>
  <h1 class="text-3xl font-bold underline text-violet-600">
    {{ hours }}:{{ minutes }}:{{ seconds }}
  </h1>
</template>