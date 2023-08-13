<script setup>
import * as Vegs from "@/assets/vegs.png";
import * as Store from "../assets/store.png";
import * as Drinks from "../assets/drinks.png";
import * as Pepper from "../assets/pepper.png";
import FeaturedCard from "./primitives/FeaturedCard.vue";
import GoodsHeader from "./primitives/GoodsHeader.vue";
</script>

<template>
  <div class="featured-wrapper">
    <GoodsHeader title="Featured Stores" />
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
.featured-wrapper {
  width: 100%;
  padding: 2rem 6rem;
}
.featured-items {
  width: 100%;
  display: flex;
  justify-content: space-between;
}
</style>
