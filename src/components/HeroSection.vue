<script setup>
import InfoLabel from "./InfoLabel.vue";
import LgText from "./primitives/typos/LgText.vue";
import XLgText from "./primitives/typos/XLgText.vue";
import SelectField from "./primitives/SelectField.vue";
import CartIcon from "./primitives/icons/CartIcon.vue";
import ActionButton from "./primitives/ActionButton.vue";
import MotorCycleIcon from "./primitives/icons/MotorCycleIcon.vue";
import LocationPin2Icon from "./primitives/icons/LocationPin2Icon.vue";
</script>

<template>
  <div class="hero">
    <div class="hero-headline">
      <div class="hero-text">
        <XLgText
          text="Local and International groceries delivered to your doorstep"
        />
        <LgText
          class="desc"
          text="Instadoor have set high standards for our stores to bring you closer to the taste of sumptuous delicacies"
        />
      </div>
    </div>
    <div class="hero-choices">
      <SelectField title="Delivering to" />
      <SelectField title="Store Type" />
      <SelectField title="Choose Dish Category" />
      <ActionButton style="height: 3rem" text="Get Food" />
    </div>
  </div>
  <div class="info-area">
    <InfoLabel :icon="LocationPin2Icon" title="Set Delivery Location">
      <p>Select the location where you want your food to be delivered to</p>
    </InfoLabel>
    <InfoLabel :icon="CartIcon" title="Choose your dish">
      <p>
        Browse through our stores near you and choose your desired groceries.
      </p>
    </InfoLabel>
    <InfoLabel :icon="MotorCycleIcon" title="Get it at your doorstep">
      <p>Wait and track your order as it will be delivered to you in no time</p>
    </InfoLabel>
  </div>
</template>

<style scoped>
.hero {
  width: 100%;
  height: 47.639%;
  padding: 8rem;
  background-size: cover;
  background-image: linear-gradient(
      90deg,
      #f73163 47.31%,
      rgba(247, 49, 99, 0) 100%
    ),
    url("../assets/rectangle.png");
}
.hero-headline {
  color: white;
}
.hero-text {
  width: 55rem;
}
.hero-text .desc {
  margin: 1rem 0;
}
.hero-choices {
  gap: 16px;
  display: flex;
  padding: 16px;
  margin: 2rem 0;
  border-radius: 8px;
  align-items: flex-end;
  background: white;
  justify-content: space-between;
}

.info-area {
  display: flex;
  bottom: 100px;
  position: relative;
  padding: 0 8rem 4rem;
  justify-content: space-between;
}
</style>
