<script setup>
defineProps(["text"]);
</script>

<template>
  <button class="action-btn">{{ text }}</button>
</template>

<style scoped>
.action-btn {
  border: none;
  width: 25%;
  color: white;
  padding: 12px 16px;
  border-radius: 8px;
  background-color: #f73163;
}
</style>
