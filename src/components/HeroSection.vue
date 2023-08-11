<script setup>
import BaseText from "./primitives/typos/BaseText.vue";
import XLgText from "./primitives/typos/XLgText.vue";
</script>

<template>
  <div class="hero">
    <div class="hero-details">
      <div class="hero-text">
        <XLgText
          text="Local and International groceries delivered to your doorstep"
        />
        <BaseText
          text="Instadoor have set high standards for our stores to bring you closer to the taste of sumptuous delicacies"
        />
      </div>
    </div>
  </div>
</template>

<style scoped>
.hero {
  width: 100%;
  height: 686px;
  padding: 8rem;
  background-size: cover;
  background-image: linear-gradient(
      90deg,
      #f73163 47.31%,
      rgba(247, 49, 99, 0) 100%
    ),
    url("../assets/rectangle.png");
}
.hero-details {
  color: white;
}
.hero-text {
  width: 55rem;
}
.hero-text desc {
  margin: 1rem;
}
</style>
