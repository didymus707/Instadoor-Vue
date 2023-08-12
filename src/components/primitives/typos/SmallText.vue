<script setup>
defineProps(["text"]);
</script>

<template>
  <p class="small-text">{{ text }}</p>
</template>

<style scoped>
.small-text {
  font-size: 12px;
  font-style: normal;
  font-weight: 400;
  line-height: 16px;
}
</style>
