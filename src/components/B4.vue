<template>
  <div
    v-bind:style="{ color: isActive ? '#fff' : 'black', background: 'blue' }"
  >
    Block
  </div>
</template>

<script setup>
const isActive = true;
</script>

<style></style>
