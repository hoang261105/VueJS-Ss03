<template>
  <div>
    <div
      :style="{ backgroundColor: changeColor, width: '200px', height: '100px' }"
    ></div>
    <button @click="handleChange">Change Background</button>
  </div>
</template>

<script setup>
import { ref } from "vue";
const changeColor = ref("red");
const handleChange = () => {
  changeColor.value = "blue";
};
</script>

<style></style>
