<template>
  <div class="wrapper">
    <SecondTaskInput v-model="title" />
    <h1>{{ title }}</h1>
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";
import SecondTaskInput from "./SecondTaskInput.vue";

export default defineComponent({
  name: "SecondTask",
  components: {
    SecondTaskInput,
  },
  data: () => ({
    title: "Title",
  }),
});
</script>
