<script setup>
import { computed } from "vue";
import StarIcon from "./icons/StarIcon.vue";
const props = defineProps({
  rating: Number,
  maxStars: { default: 5, type: Number },
});

const computedRating = computed(() => Math.min(props.rating, props.maxStars));
</script>

<template>
  <div class="rating">
    <span v-for="(star, index) in maxStars" :key="index" class="star">
      <StarIcon />
    </span>
  </div>
</template>

<style scoped>
.rating {
  display: flex;
  align-items: center;
}
.star {
  display: flex;
}
</style>
