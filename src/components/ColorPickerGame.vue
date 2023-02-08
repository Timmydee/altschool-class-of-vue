
<template>
  <h1>Color Picker Game</h1>

  <div>{{ message }}</div>

  <button v-for="color in colors" :key="color" @click="matchColor(color)">
    {{ color }}
  </button>
</template>

<script setup>
import {ColorGame} from '../composables/ColorGame.js'

const { colors, message, matchColor } = ColorGame()

</script>

<style></style>
