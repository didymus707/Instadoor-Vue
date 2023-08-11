<script setup>
defineProps(["text"]);
</script>

<template>
  <span class="text-base">{{ text }}</span>
</template>

<style scoped>
.text-base {
  font-size: 16px;
  font-style: normal;
  font-weight: 400;
  line-height: 24px;
}
</style>
