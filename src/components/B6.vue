<template>
  <button @click="handleClick('Rikkei Academy')">Get Param</button>
</template>

<script setup>
const handleClick = (message) => {
  console.log(message);
};
</script>

<style></style>
