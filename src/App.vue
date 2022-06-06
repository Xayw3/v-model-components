<template>
  <FirstTask />
  <SecondTask />
  <ThirdTask />
  <FourthTask />
  <FifthTask />
  <SixthTask />
  <SeventhTask />
  <EighthTask />
</template>

<script lang="ts">
import { defineComponent } from "vue";
import FirstTask from "./components/FirstTask/FirstTask.vue";
import SecondTask from "./components/SecondTask/SecondTask.vue";
import ThirdTask from "./components/ThirdTask/ThirdTask.vue";
import FourthTask from "./components/FourthTask/FourthTask.vue";
import FifthTask from "./components/FifthTask/FifthTask.vue";
import SixthTask from "./components/SixthTask/SixthTask.vue";
import SeventhTask from "./components/SeventhTask/SeventhTask.vue";
import EighthTask from "./components/EighthTask/EighthTask.vue";

export default defineComponent({
  name: "HomeView",
  components: {
    FirstTask,
    SecondTask,
    ThirdTask,
    FourthTask,
    FifthTask,
    SixthTask,
    SeventhTask,
    EighthTask,
  },
});
</script>

<style lang="scss">
.box {
  width: 50px;
  height: 50px;
  border: 1px solid #333;
  background-color: red;
}

.hidden {
  visibility: hidden;
}

.wrapper {
  max-width: 800px;
  border: 1px solid #333;
  display: flex;
  align-items: center;
  padding: 10px;
  justify-content: space-between;
  margin: 15px;
}

.wrapper-column {
  flex-direction: column;
  gap: 5px;
}

.margin-right {
  margin-right: 15px;
}
</style>
