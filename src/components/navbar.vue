<script setup>
import { ref } from "vue";
import LogoIcon from "./primitives/icons/LogoIcon.vue"
import BaseText from './primitives/typos/BaseText.vue'
const isBold = ref(true);
</script>

<template>
  <template class="wrapper">
    <div class="logo">
      <LogoIcon />
    </div>
    <nav class="navlinks">
      <ul>
        <li><a href="#" class="active">Home</a></li>
        <li><a href="#">Partners</a></li>
        <li><a href="#">Courier</a></li>
        <li><a href="#">FAQ</a></li>
        <li><a href="#">About Us</a></li>
        <li><a href="#">Contact Us</a></li>
      </ul>
    </nav>
    <div class="cta">
      <button class="btn-cta">
        <BaseText text="Sign In" />
      </button>
      <button class="btn-cta btn-cta-signup">
        <BaseText :class="isBold ? 'is-bold' : 'is-normal'" text="Sign Up" />
      </button>
    </div>
  </template>
</template>

<style scoped>
.wrapper {
  width: 100%;
  display: flex;
  padding: 12px 128px;
  align-items: center;
  background-color: #343a40;
  justify-content: space-between;
}
.logo {
  display: flex;
  align-items: center;
}
.navlinks {
  width: 40%;
}
.navlinks ul {
  padding: 0;
  width: 100%;
  display: flex;
  list-style-type: none;
  justify-content: space-between;
}
.navlinks a {
  color: white;
  text-decoration: none;
}
.navlinks .active {
  color: #f73163;
}
.cta {
  gap: 1rem;
  display: flex;
  align-items: center;
  justify-content: center;
}
.btn-cta {
  padding: 0.5rem;
  border: none;
  color: white;
  background: none;
}
.btn-cta-signup {
  color: #f73163;
  border-radius: 8px;
  border: 1px solid #f73163;
}
.is-bold {
  font-weight: 600;
}

.is-normal {
  font-weight: 400;
}
</style>
