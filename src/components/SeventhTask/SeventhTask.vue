<template>
  <div class="wrapper">
    <SeventhTaskButton v-model:toggle="isActive" />
    <div class="box" :class="[isActive ? '' : 'hidden']"></div>
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";
import SeventhTaskButton from "./SeventhTaskButton.vue";

export default defineComponent({
  name: "SecondTask",
  components: {
    SeventhTaskButton,
  },
  data: () => ({
    isActive: true,
  }),
});
</script>
