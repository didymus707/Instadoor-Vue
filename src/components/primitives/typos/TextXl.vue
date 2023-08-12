<script setup>
defineProps(["text"]);
</script>

<template>
  <h1 class="text-xl">
    {{ text }}
  </h1>
</template>

<style scoped>
.text-sl {
  font-size: 4rem;
  font-style: normal;
  font-weight: 700;
  line-height: 4.5rem;
  letter-spacing: 1px;
}
</style>
