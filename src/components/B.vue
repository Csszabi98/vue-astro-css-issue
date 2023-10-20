<template>
  <div class="component-b">
    <span>Component B</span>
    <A />
  </div>
</template>

<script setup>
  import { defineAsyncComponent } from 'vue';

  const A = defineAsyncComponent(() => import('./A.vue'));
</script>

<style>
  .component-b {
    border: 1px solid blue;
    padding: 12px;
  }
</style>
