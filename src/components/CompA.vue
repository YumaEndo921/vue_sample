

<script setup>
import CompB from './CompB.vue';
import { counter } from '../store/countStore';
</script>
<template>
  <h2>CompAコンポーネント</h2>
  <p>Count:{{ counter.count }}</p>
   <CompB  />
</template>