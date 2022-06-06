<template>
  <div class="wrapper">
    <FourthTaskInput v-model="color" />
    <div class="box" :style="{ backgroundColor: color }"></div>
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";
import FourthTaskInput from "./FourthTaskInput.vue";

export default defineComponent({
  name: "SecondTask",
  components: {
    FourthTaskInput,
  },
  data: () => ({
    color: "",
  }),
});
</script>
