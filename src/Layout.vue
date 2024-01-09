<script setup lang="ts">
import { reactive } from 'vue';
import PokemonTimePlayed from './widgets/PokemonTimePlayed.vue'
import { GenericClient } from '@gamehook-io/client';

const client = reactive(new GenericClient())
await client.connect()
</script>

<template>
  <PokemonTimePlayed :client="client" />
</template>