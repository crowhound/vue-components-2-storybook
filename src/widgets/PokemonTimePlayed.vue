<script setup lang="ts">
import { GenericClient } from '@gamehook-io/client';

import Timer from '../components/Timer.vue'

defineProps<{
  client: GenericClient
}>()
</script>
<template>
    <Timer :hours="client.values.gameTime.hours" :minutes="client.values.gameTime.minutes" :seconds="client.values.gameTime.seconds" />
</template>