

<script setup>
import { ref, reactive, computed } from 'vue';
const count = ref(0);

// const clickButton = ()=>{
//   count ++
// }

const user = reactive({
  firstName: 'John',
  lastName: 'Doe',
});

const fullName = () => {
  console.log('Function');
  return `${user.firstName} ${user.lastName}`;
};
const cFullName = computed(() => {
  console.log('Computed Propety');
  return `${user.firstName} ${user.lastName}`;
});
</script>

<template>
  <h1>Vue 3 入門</h1>
  <h2>fullName: {{ fullName() }}</h2>
  <h2>cFullName: {{ cFullName }}</h2>
  <!-- <input v-model="user.firstName" /> -->
  <button @click="count++">count is : {{ count }}</button>

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
