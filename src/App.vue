
<script setup>
const stock = 6;
</script>

<template>
  <h1>Vue 3 入門</h1>
  <div v-if="stock > 5 " >まだ商品に在庫数に余裕があります</div>
  <div v-else-if="stock === 0">申し訳ございません。現在売り切れです。</div>
  <div v-else>在庫数が少なくなっています。お急ぎください。</div>
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
