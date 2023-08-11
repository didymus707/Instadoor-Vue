<script setup>
import TextLg from "./primitives/typos/TextXL.vue";
</script>

<template>
  <div class="hero">
    <div class="hero-details">
      <TextLg
        text="Local and International groceries delivered to your doorstep"
      />

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
</style>
