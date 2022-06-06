<template>
  <div class="wrapper">
    <EighthTaskCheckbox v-model:toggle="isActive" />
    <div class="box" :class="[isActive ? '' : 'hidden']"></div>
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";
import EighthTaskCheckbox from "./EighthTaskCheckbox.vue";

export default defineComponent({
  name: "SecondTask",
  components: {
    EighthTaskCheckbox,
  },
  data: () => ({
    isActive: true,
  }),
});
</script>
