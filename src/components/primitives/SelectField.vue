<script setup>
import { ref } from "vue";
import BaseText from "./typos/BaseText.vue";
import PinLocation from "./icons/PinLocation.vue";
const props = defineProps({
  options: Array,
  title: String,
});
const text = ref("");
const options = ["vegetables", "pepper", "soaps & detergents"];
console.log(props);
</script>

<template>
  <div class="select-field-wrapper">
    <BaseText class="isBold" :text="title" />
    <div class="dropdown-wrapper">
     <PinLocation v-if="title === 'Delivering to'" class="dropdown-icon margin-right" />
      <input class="delivering" v-if="title === 'Delivering to'" v-model="text" type="text" />
      <Select v-else class="dropdown-select">
        <option value="">Select type</option>
        <option v-for="item in options" :key="item" :value="item">
          {{ item }}
        </option>
      </Select>
    </div>
  </div>
</template>

<style scoped>
.select-field-wrapper {
  width: 25%;
}
.dropdown-wrapper {
  display: flex;
  height: 3rem;
  padding: 12px;
  border-radius: 4px;
  align-items: center;
  background: #f1f3fb;
  justify-content: space-between;
  border: 0.5px solid #e3e5e8;
}
.delivering {
  width: 89%;
  border: none;
  font-size: 1rem;
  color: #737D8C;
  background: #f1f3fb;
}
.dropdown-select {
  border: none;
  width: 100%;
  font-size: 1rem;
  color: #737D8C;
  background: #f1f3fb;
}
.dropdown-icon {
  width: 24px;
  height: 24px;
}
.margin-right {
  margin-right: 8px;
}
.isBold {
  font-weight: 600;
  margin-bottom: 8px;
  color: #171a1c;
}
</style>
