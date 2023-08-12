<script setup>
const props = defineProps({
  icon: Object,
  title: String,
});
</script>

<template>
  <div class="info-label-wrapper">
    <div class="icon-container">
      <component :is="icon" />
    </div>
    <LgText class="bold">{{ title }}</LgText>
    <BaseText :class="color"><slot /></BaseText>
  </div>
</template>

<style scoped>
.info-label-wrapper {
  width: 30%;
  display: flex;
  padding: 24px;
  border-radius: 8px;
  flex-direction: column;
  align-items: flex-start;
  background: #fff5f8;
}
.bold {
  font-weight: 600;
  margin-top: 1rem;
  margin-bottom: 8px;
  color: #F73163;
}
.color {
  color:#171A1C
}
</style>
