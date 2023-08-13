<script setup>
import * as Pic from "@/assets/pic.png";
import LgText from "./primitives/typos/LgText.vue";
import BigLgText from "./primitives/typos/BigLgText.vue";
</script>
<template>
  <div class="quick-info">
    <div class="quick-info-content">
      <img :src="Pic.default" alt="" class="pic-img" />
      <div class="content-words">
        <BigLgText
          style="margin-bottom: 1rem"
          text="Today, more and more people want the convenience of delivery"
        />
        <LgText
          text="Get quick and fast access to groceries from your favorite store today"
        />
      </div>
    </div>
  </div>
</template>

<style scoped>
.quick-info {
  padding: 2rem 6rem;
}
.quick-info-content {
  width: 100%;
  display: flex;
  /* border-radius: 8px; */
}

.pic-img,
.content-words {
  width: 50%;
}
.pic-img {
  /* background: 50% / cover no-repeat #f73163; */
  background: linear-gradient(90deg, rgba(255,255,255,1) 50%, rgba(247,49,99,1) 52%);
}
.content-words {
  padding: 5.25rem;
  color: white;
  background: #f73163;
  border-top-right-radius: 1rem;
  border-bottom-right-radius: 1rem;
}
</style>
