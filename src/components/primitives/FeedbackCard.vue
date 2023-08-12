<script setup>
import BaseText from "./typos/BaseText.vue";
import * as Avatar from "../../assets/avatar.png";
</script>

<template>
  <div class="feedback-card-wrapper">
    <div class="feedback-text">
      <BaseText
        text="Lorem ipsum dolor sit amet, consectetur adipiscing elit. Molestie sem scelerisque diam arcu nisl magna diam scelerisque. In nunc, placerat suscipit gravida ac aenean sapien. Quis tincidunt tempus pulvinar tristique aenean fusce. Blandit magna sem amet varius."
      />
    </div>
    <div class="feedback-user">
      <img :src="Avatar.default" alt="User Avatar" />
      <div class="feedback-name">
        <BaseText style="font-weight: 600" text="Naila Nkechinyere" />
        <BaseText style="font-size: 14px" text="Enterpreneur" />
      </div>
    </div>
  </div>
</template>

<style scoped>
.feedback-card-wrapper {
  gap: 16px;
  width: 30%;
  display: flex;
  padding: 24px;
  flex-direction: column;
  align-items: flex-start;
  border-radius: 16px;
  background: #fff5f8;
}
.feedback-user {
  display: flex;
  margin-top: 1rem;
}
.feedback-name {
  margin-left: 1rem;
}
</style>
