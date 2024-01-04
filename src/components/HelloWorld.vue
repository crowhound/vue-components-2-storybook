<script setup lang="ts">
defineProps<{
  values: any
}>()
</script>

<template>
  <h1 class="text-3xl font-bold underline text-violet-600">
    Hello {{ values.player.name }}
  </h1>
</template>