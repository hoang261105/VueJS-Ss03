<template>
  <a href="#" @click.stop.prevent="doThat">Click</a>
</template>

<script setup>
const link = "http://www.google.com";

// Hàm kiểm tra tính hợp lệ của URL
const isValidURL = (url) => {
  try {
    new URL(url);
    return true;
  } catch (error) {
    return false;
  }
};

const doThat = () => {
  if (isValidURL(link)) {
    window.location.href = link;
  } else {
    alert("Đường dẫn không hợp lệ");
  }
};
</script>

<style></style>
