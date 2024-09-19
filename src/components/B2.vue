<template>
  <div>
    <h1 v-bind="name">Heading</h1>
  </div>
</template>

<script setup>
const name = {
  elementId: "heading",
  elementClass: "heading",
};
</script>

<style></style>
