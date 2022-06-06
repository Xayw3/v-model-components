<template>
  <div class="wrapper">
    <SixthTaskInput v-model:model-title="title" v-model:model-desc="desc" />
    <SixthTaskText :title="title" :desc="desc" />
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";
import SixthTaskInput from "./SixthTaskInput.vue";
import SixthTaskText from "./SixthTaskText.vue";

export default defineComponent({
  name: "SixthTask",
  components: {
    SixthTaskInput,
    SixthTaskText,
  },
  data: () => ({
    title: "Title",
    desc: "Description",
  }),
});
</script>
