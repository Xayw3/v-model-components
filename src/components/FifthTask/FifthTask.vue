<template>
  <div class="wrapper wrapper-column">
    <FifthTaskInput v-model:model-title="title" v-model:model-desc="desc" />
    <FifthTaskText :title="title" :desc="desc" />
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";
import FifthTaskInput from "./FifthTaskInput.vue";
import FifthTaskText from "./FifthTaskText.vue";

export default defineComponent({
  name: "FifthTask",
  components: {
    FifthTaskInput,
    FifthTaskText,
  },
  data: () => ({
    title: "",
    desc: "",
  }),
});
</script>
