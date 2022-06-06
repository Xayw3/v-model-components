<template>
  <label>
    <input :checked="active" type="checkbox" @click="handleGetValue" />
    {{ active ? "hide box" : "show box" }}
  </label>
</template>

<script lang="ts">
import { defineComponent } from "vue";

export default defineComponent({
  name: "EighthTaskInput",
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
