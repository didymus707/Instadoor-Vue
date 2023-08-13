<script setup>
import * as Peas from "@/assets/peas.png";
import * as Broc from "@/assets/broc.png";
import * as Onion from "@/assets/onion.png";
import * as Green from "@/assets/green.png";
import * as Tomato from "@/assets/tomato.png";
import * as Yelcarr from "@/assets/yelcarr.png";
import * as Rcarpep from "@/assets/rcarpep.png";
import * as YrPepper from "@/assets/yr-pepper.png";
import GoodsHeader from "./primitives/GoodsHeader.vue";
import RecommendedCard from "./primitives/RecommendedCard.vue";
const foodArr = [
  {
    image: YrPepper,
    price: 50,
    oldPrice: 60,
    timeRange: "30 -60 mins",
    foodName: "Nigerian Breakfast",
  },
  {
    image: Broc,
    price: 50,
    oldPrice: 60,
    timeRange: "30 -60 mins",
    foodName: "Nigerian Breakfast",
  },
  {
    image: Green,
    price: 50,
    oldPrice: 60,
    timeRange: "30 -60 mins",
    foodName: "Nigerian Breakfast",
  },
  {
    image: Yelcarr,
    price: 50,
    oldPrice: 60,
    timeRange: "30 -60 mins",
    foodName: "Nigerian Breakfast",
  },
  {
    image: Rcarpep,
    price: 50,
    oldPrice: 60,
    timeRange: "30 -60 mins",
    foodName: "Nigerian Breakfast",
  },
  {
    image: Tomato,
    price: 50,
    oldPrice: 60,
    timeRange: "30 -60 mins",
    foodName: "Nigerian Breakfast",
  },
  {
    image: Peas,
    price: 50,
    oldPrice: 60,
    timeRange: "30 -60 mins",
    foodName: "Nigerian Breakfast",
  },
  {
    image: Onion,
    price: 50,
    oldPrice: 60,
    timeRange: "30 -60 mins",
    foodName: "Nigerian Breakfast",
  },
];
</script>

<template>
  <div class="recommended-wrapper">
    <GoodsHeader title="Recommendation" />
    <div class="recommended-items">
      <RecommendedCard
        v-for="foodItem in foodArr"
        :key="foodItem.foodName"
        :image="foodItem.image"
        :price="foodItem.price"
        :oldPrice="foodItem.oldPrice"
        :timeRange="foodItem.timeRange"
        :foodName="foodItem.foodName"
      />
    </div>
  </div>
</template>

<style scoped>
.recommended-wrapper {
  width: 100%;
  padding: 2rem 6rem;
}
.recommended-items {
  width: 100%;
  row-gap: 32px;
  display: flex;
  flex-wrap: wrap;
  justify-content: space-between;
}
</style>
