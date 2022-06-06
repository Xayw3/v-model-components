<template>
  <div class="wrapper wrapper-column">
    <input type="text" v-model="title" />
    <button @click="setTitle">Change title</button>
  </div>
  <div class="wrapper wrapper-column">
    <input type="text" v-model="desc" />
    <button @click="setDesc">Change description</button>
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";

export default defineComponent({
  name: "SixthTaskInput",
  props: ["modelTitle", "modelDesc"],
  emits: ["update:modelTitle", "update:modelDesc"],
  data: () => ({
    title: "",
    desc: "",
  }),
  methods: {
    setTitle() {
      this.$emit("update:modelTitle", this.title);
    },
    setDesc() {
      this.$emit("update:modelDesc", this.desc);
    },
  },
});
</script>
