
<script setup>
const clickButton = (msg) => {
  console.log(msg);
};
const another = (msg) => {
  console.log(msg);
};
</script>

<template>
  <h1>Vue 3 入門</h1>
  <button @click="clickButton('クリック'), another('click')">クリック</button>
</template>

<style scoped>
.active {
  color: red;
  font-weight: 900;
}
.underLine {
  text-decoration: underline;
}
.back {
  background-color: black;
}
</style>
