<template>
  <h2>title: {{ title }}</h2>
  <h2>description: {{ desc }}</h2>
</template>

<script lang="ts">
import { defineComponent } from "vue";

export default defineComponent({
  name: "FifthTaskText",
  props: ["title", "desc"],
});
</script>
