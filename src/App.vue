<script>
import ColorPickerGame from "./components/ColorPickerGame.vue";


export default {
  components: { ColorPickerGame},
  data() {
    return {
      currentLesson: "color-picker-game",
    };
  },
};
</script>

<template>
  <ColorPickerGame v-if="currentLesson === 'color-picker-game'" />
</template>

<style scoped></style>
