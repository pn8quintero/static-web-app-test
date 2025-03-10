<script setup lang="ts">
defineProps<{ msg: string }>();
const htmlContent = import.meta.env.VITE_HTML_CONTENT || "";
</script>

<template>
  <h1>{{ msg }}</h1>

  <div v-html="htmlContent"></div>
</template>

<style scoped>
.read-the-docs {
  color: #888;
}
</style>
