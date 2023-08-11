<script setup>
defineProps(["text"]);
</script>

<template>
  <h1 class="x-large">{{ text }}</h1>
</template>

<style scoped>
.x-large {
  font-size: 64px;
  font-style: normal;
  font-weight: 700;
  line-height: 72px;
  letter-spacing: 1px;
}
</style>
