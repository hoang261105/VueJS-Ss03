<template>
  <input type="text" @input="handleChange" @keydown.enter="handleEnter" />
</template>

<script setup>
import { ref } from "vue";
const inputText = ref("");
const handleChange = (e) => {
  inputText.value = e.target.value;
};

const handleEnter = () => {
  alert(inputText.value);
};
</script>

<style></style>
