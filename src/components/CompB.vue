

<script setup>
import { counter } from '../store/countStore';
</script>

<template>
  <h3>CompBコンポーネント</h3>
  <p>{{ message }}</p>
  <p>Count :{{ counter.count }}</p>
  <button @click="counter.addCount">+</button>
</template>