<template>
  <div>
    <form action="" @submit.prevent="onSubmit">
      <input type="text" />
      <button type="submit">Submit</button>
    </form>
  </div>
</template>

<script setup>
const onSubmit = () => {
  console.log("Form submitted");
};
</script>

<style></style>
