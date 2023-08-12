<script setup>
defineProps(["title"]);
import BaseText from './typos/BaseText.vue';
import BigLgText from './typos/BigLgText.vue';
import RightCaretIcon from './icons/RightCaretIcon.vue';
</script>

<template>
  <div class="featured-header">
    <BigLgText :text="title" />
    <div class="see-all">
      <BaseText class="bold" text="See All" />
      <RightCaretIcon />
    </div>
  </div>
</template>

<style scoped>
.featured-header {
  display: flex;
  margin-bottom: 1rem;
  align-items: center;
  justify-content: space-between;
}
.see-all {
  display: flex;
}
.bold {
  font-weight: 600;
  margin-right: 8px;
  color: black;
}
</style>
