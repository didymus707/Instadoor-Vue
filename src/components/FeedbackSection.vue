<script setup>
import BaseText from "./primitives/typos/BaseText.vue";
import FeedbackCard from "./primitives/FeedbackCard.vue";
import BigLgText from "./primitives/typos/BigLgText.vue";
</script>

<template>
  <div class="feedback-container">
    <div class="feedback-header">
      <BigLgText style="margin-bottom: 8px" text="Happy Customers" />
      <BaseText
        style="font-weight: 600; margin-bottom: 2rem"
        text="Our Customers are full of praise for Instadoor"
      />
    </div>
    <div class="feedback-card-wrapper">
      <FeedbackCard />
      <FeedbackCard />
      <FeedbackCard />
    </div>
  </div>
</template>

<style scoped>
.feedback-card-wrapper {
  display: flex;
  justify-content: space-between;
}
</style>
