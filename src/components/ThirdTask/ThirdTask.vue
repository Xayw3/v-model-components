<template>
  <div class="wrapper">
    <ThirdTaskInput v-model="color" />
    <div class="box" :style="{ backgroundColor: color }"></div>
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";
import ThirdTaskInput from "./ThirdTaskInput.vue";

export default defineComponent({
  name: "SecondTask",
  components: {
    ThirdTaskInput,
  },
  data: () => ({
    color: "",
  }),
});
</script>
