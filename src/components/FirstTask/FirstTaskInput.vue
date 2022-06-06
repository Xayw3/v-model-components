<template>
  <input type="text" v-model="value" />
</template>

<script lang="ts">
import { defineComponent } from "vue";

export default defineComponent({
  name: "FirstTaskInput",
  props: ["modelValue"],
  emits: ["update:modelValue"],
  computed: {
    value: {
      get() {
        return this.modelValue;
      },
      set(value: HTMLInputElement) {
        this.$emit("update:modelValue", value);
      },
    },
  },
});
</script>
