<template>
  <div class="demo">
    <PokeBall />
    <PokeBall :size="80" :speed="0.8" />
    <PokeBall :size="160" :speed="2" />
  </div>
</template>

<script setup lang="ts">
import { PokeBall } from './index'
</script>

<style scoped>
.demo {
  display: flex;
  gap: 40px;
  padding: 40px;
}
</style>
