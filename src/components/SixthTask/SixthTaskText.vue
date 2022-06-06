<template>
  <h2 class="margin-right">{{ title }}</h2>
  <h2>{{ desc }}</h2>
</template>

<script lang="ts">
import { defineComponent } from "vue";

export default defineComponent({
  name: "SixthTaskText",
  props: ["title", "desc"],
});
</script>
