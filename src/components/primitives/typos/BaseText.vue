<script setup>
defineProps(["text"]);
</script>

<template>
  <p class="text-base">{{ text }}</p>
</template>

<style scoped>
.text-base {
  font-size: 16px;
  font-style: normal;
  font-weight: 400;
  line-height: 24px;
}
</style>
