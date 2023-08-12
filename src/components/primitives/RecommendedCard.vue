<script setup>
import BaseText from "./typos/BaseText.vue";
import SmallText from "./typos/SmallText.vue";
import ActionButton from "./ActionButton.vue";
const props = defineProps({
  image: Object,
  price: Number,
  oldPrice: Number,
  foodName: String,
  timeRange: String,
});

</script>

<template>
  <div class="recommended-card">
    <div class="image">
      <img :src="image.default" alt="food Image" />
    </div>
    <div class="reco-desc">
      <BaseText :text="foodName" />
      <BaseText class="bold" :text="`${'$' + ' ' + price}`" />
      <div class="price-time">
        <SmallText class="strike" :text="`${'$' + ' ' + oldPrice}`" />
        <SmallText class="time-range" :text="timeRange" />
      </div>
      <ActionButton style="width: 100%" text="Add to Cart" />
    </div>
  </div>
</template>

<style scoped>
.recommended-card {
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
.reco-desc {
  gap: 8px;
  width: 100%;
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  padding: 8px 24px 24px 24px;
}

.price-time {
  width: 100%;
  display: flex;
  align-items: center;
  justify-content: space-between;
}
.bold {
  font-weight: 600;
}
.strike {
  text-decoration: line-through;
}
.time-range {
  color: #f73163;
}
</style>
