<script setup>
defineProps(["text"]);
</script>

<template>
  <h1 class="text-xl">{{ text }}</h1>
</template>

<style scoped>
.text-xl {
  font-family: Inter;
  font-size: 64px;
  font-style: normal;
  font-weight: 700;
  line-height: 72px; /* 112.5% */
  letter-spacing: 1px;
}
</style>
