<script setup>
defineProps(["text"]);
</script>

<template>
  <span class="text-xsmall">{{ text }}</span>
</template>

<style scoped>
.text-xsmall {
  font-size: 8px;
  font-style: normal;
  font-weight: 400;
  line-height: 24px;
}
</style>
