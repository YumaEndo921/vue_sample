

<script setup>
import { reactive, computed } from 'vue';
const user = reactive({
  firstName: 'John',
  lastName: 'Doe',
});
const fullName = () => `${Math.random()} ${user.firstName} ${user.lastName}`;
const cFullName = computed(
  () => `${Math.random()} $${user.firstName} ${user.lastName}`
);
</script>

<template>
  <h1>Vue 3 入門</h1>
  <h2>fullName: {{ fullName() }}</h2>
  <h2>fullName: {{ fullName() }}</h2>
  <h2>fullName: {{ fullName() }}</h2>
  <h2>cFullName: {{ cFullName }}</h2>
  <h2>cFullName: {{ cFullName }}</h2>
  <h2>cFullName: {{ cFullName }}</h2>
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
