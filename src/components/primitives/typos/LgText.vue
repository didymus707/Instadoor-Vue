<script setup>
defineProps(["text"]);
</script>

<template>
  <h3 class="lg-text">{{ text }}</h3>
</template>

<style scoped>
.lg-text {
  font-size: 1.5rem;
  font-style: normal;
  font-weight: 500;
  line-height: 2rem;
}
</style>
