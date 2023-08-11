<script setup>
defineProps(["text"]);
</script>

<template>
  <span class="text-small">{{ text }}</span>
</template>

<style scoped>
.text-small {
  font-size: 12px;
  font-style: normal;
  font-weight: 400;
  line-height: 24px;
}
</style>
