<template>
  <h1>Color Picker Game</h1>

  <div>{{ message }}</div>

  <button v-for="color in colors" :key="color" @click="matchColor(color)">
    {{ color }}
  </button>
</template>

<script>
// import { ref, reactive } from "@vue/reactivity";
import { useColorPickerGame } from '../composable/useColorPickerGame.js'
export default {
  setup() {
    const { colors, message, matchColor } = useColorPickerGame()
    return { colors, message, matchColor };
  },
};
</script>

<style>
</style>
