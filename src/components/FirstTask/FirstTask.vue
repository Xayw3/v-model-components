<template>
  <div class="wrapper">
    <FirstTaskInput v-model="title" />
    <h1>{{ title }}</h1>
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";
import FirstTaskInput from "./FirstTaskInput.vue";

export default defineComponent({
  name: "FirstTask",
  components: {
    FirstTaskInput,
  },
  data: () => ({
    title: "",
  }),
});
</script>
