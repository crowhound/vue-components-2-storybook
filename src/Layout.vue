<script setup lang="ts">
import { reactive } from 'vue';
import HelloWorld from './components/HelloWorld.vue'
import { GenericClient } from '@gamehook-io/client';

const client = reactive(new GenericClient())
await client.connect()
</script>

<template>
  <HelloWorld :values="client.values" />
</template>