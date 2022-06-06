<template>
  <button @click="handleGetValue">
    {{ active ? "hide box" : "show box" }}
  </button>
</template>

<script lang="ts">
import { defineComponent } from "vue";

export default defineComponent({
  name: "SeventhTaskInput",
  data: () => ({
    active: true,
  }),
  props: ["toggle"],
  emits: ["update:toggle"],
  methods: {
    handleGetValue() {
      this.active = !this.active;

      this.$emit("update:toggle", this.active);
    },
  },
});
</script>
