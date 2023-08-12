<script setup>
const props = defineProps({
  text: String,
});
</script>

<template>
  <p class="big-lg-text">{{ text }}</p>
</template>

<style scoped>
.big-lg-text {
  font-family: Inter;
  font-size: 2rem;
  font-style: normal;
  font-weight: 700;
  line-height: 40px;
}
</style>
