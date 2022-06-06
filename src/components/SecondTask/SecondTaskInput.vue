<template>
  <div class="wrapper">
    <input class="margin-right" type="text" v-model="value" />
    <button @click="setValue">Change text</button>
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";

export default defineComponent({
  name: "SecondTaskInput",
  props: ["modelValue"],
  emits: ["update:modelValue"],
  data: () => ({
    value: "",
  }),
  methods: {
    setValue() {
      this.$emit("update:modelValue", this.value);
    },
  },
});
</script>
