<template>
  <div
    class="pokeball"
    :style="{
      '--size': size + 'px',
      '--speed': speed + 's'
    }"
  />
</template>

<script setup lang="ts">
import './poke-ball.css'

/**
 * 精灵球组件 Props
 * size  : 控制整体大小（px）
 * speed : 控制动画周期（秒，越小越快）
 */
const props = withDefaults(
  defineProps<{
    size?: number
    speed?: number
  }>(),
  {
    size: 120,
    speed: 1.5
  }
)
</script>

<script lang="ts">
export default {
  name: 'PokeBall'
}
</script>
