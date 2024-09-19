<template>
  <div>
    <img v-bind:src="image" alt="" width="200px" height="100px" />
    <br />
    <button @click="handleChange">Change Image</button>
  </div>
</template>

<script setup>
import { ref } from "vue";
const listImage = [
  "https://d1hjkbq40fs2x4.cloudfront.net/2017-08-21/files/landscape-photography_1645.jpg",
  "https://images2.thanhnien.vn/528068263637045248/2024/1/25/e093e9cfc9027d6a142358d24d2ee350-65a11ac2af785880-17061562929701875684912.jpg",
  "https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTvNPfCI7nzUNGhPDTL_HT5tmIkA3ssVZFuGA&s",
  "https://data.webnhiepanh.com/wp-content/uploads/2020/11/21105453/phong-canh-1.jpg",
];
const image = ref(listImage[0]);

const handleChange = () => {
  const randomIndex = Math.floor(Math.random() * listImage.length);
  image.value = listImage[randomIndex];
};
</script>

<style></style>
