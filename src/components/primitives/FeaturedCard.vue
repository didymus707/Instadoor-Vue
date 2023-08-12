<script setup>
import LgText from "./typos/LgText.vue";
import BaseText from "./typos/BaseText.vue";
import SmallText from "./typos/SmallText.vue";
import Ratings from "./Ratings.vue";
const props = defineProps({
  image: Object,
  rating: Number,
  address: String,
  timeAway: String,
  storeName: String,
});
</script>

<template>
  <div class="featured-card">
    <div class="image">
      <img :src="image.default" alt="Store Image" />
    </div>
    <div class="image-desc">
      <LgText class="image-desc-head" :text="storeName" />
      <BaseText style="font-size: 14px" :text="address" />
      <div class="time-ratings">
        <SmallText style="color: #737d8c" :text="timeAway" />
        <Ratings :rating="rating" />
      </div>
    </div>
  </div>
</template>

<style scoped>
.featured-card {
  width: 23%;
  display: flex;
  border-radius: 8px;
  flex-direction: column;
  align-items: flex-start;
  border: 1px solid #e3e5e8;
}
.image,
img {
  width: 100%;
  border-top-left-radius: 8px;
  border-top-right-radius: 8px;
}
.image-desc {
  gap: 8px;
  width: 100%;
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  padding: 8px 24px 24px 24px;
}
.image-desc-head {
  margin: 8px 0 4px;
}
.time-ratings {
  width: 100%;
  display: flex;
  align-items: center;
  justify-content: space-between;
}
</style>
