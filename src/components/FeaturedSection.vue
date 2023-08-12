<script setup>
import BigLgText from "./primitives/typos/BigLgText.vue";
import BaseText from "./primitives/typos/BaseText.vue";
import FeaturedCard from "./primitives/FeaturedCard.vue";
import RightCaretIcon from "./primitives/icons/RightCaretIcon.vue";
import * as Vegs from "@/assets/vegs.png";
import * as Store from "../assets/store.png";
import * as Drinks from "../assets/drinks.png";
import * as Pepper from "../assets/pepper.png";
</script>

<template>
  <div class="featured-wrapper">
    <div class="featured-header">
      <BigLgText text="Featured Section" />
      <div class="see-all">
        <BaseText class="bold" text="See All" />
        <RightCaretIcon />
      </div>
    </div>
    <div class="featured-items">
      <FeaturedCard
        ratings="5"
        :image="Store"
        timeAway="45 mins Away"
        storeName="Village Bukka"
        address="Location Address"
      />
      <FeaturedCard
        ratings="4"
        :image="Drinks"
        timeAway="45 mins Away"
        storeName="Village Bukka"
        address="Location Address"
      />
      <FeaturedCard
        ratings="2"
        :image="Vegs"
        timeAway="45 mins Away"
        storeName="Village Bukka"
        address="Location Address"
      />
      <FeaturedCard
        ratings="5"
        :image="Pepper"
        timeAway="45 mins Away"
        storeName="Village Bukka"
        address="Location Address"
      />
    </div>
  </div>
</template>

<style scoped>
.fetaured-wrapper {
  widows: 100%;
  padding: 2rem 8rem;
}

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
.featured-items {
  width: 100%;
  display: flex;
  justify-content: space-between;
}
</style>
