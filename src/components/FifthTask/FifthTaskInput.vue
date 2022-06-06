<template>
  <div class="wrapper">
    <input
      placeholder="change title"
      class="margin-right"
      type="text"
      v-model="title"
    />
    <input placeholder="change description" type="text" v-model="desc" />
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";

export default defineComponent({
  name: "FifthTaskInput",
  props: ["modelTitle", "modelDesc"],
  emits: ["update:modelTitle", "update:modelDesc"],
  computed: {
    title: {
      get() {
        return this.modelTitle;
      },
      set(title: HTMLInputElement) {
        this.$emit("update:modelTitle", title);
      },
    },
    desc: {
      get() {
        return this.modelDesc;
      },
      set(desc: HTMLInputElement) {
        this.$emit("update:modelDesc", desc);
      },
    },
  },
});
</script>
