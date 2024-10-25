<template>
  <header>
    <!-- <div class="wrapper">
      <nav>
        <RouterLink to="/categories">Category</RouterLink>
        <RouterLink to="/promotions">Promotions</RouterLink>
        <RouterLink to="/products">Products</RouterLink>
      </nav>
    </div> -->
    <div class="C">
      <category-component />
      <Promotion />
      <Products />
    </div>
  </header>
  <!-- <RouterView /> -->
</template>

<script setup>
import { RouterLink, RouterView } from "vue-router";
import CategoryComponent from "./views/Categories.vue";
import Promotion from "./views/Promotions.vue";
import Products from "./views/Products.vue";
</script>

<style scoped>
.C {
  height: 120vh;
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  gap: 1rem;
}
/* .wrapper {
  padding: 20px;
  background-color: #f8f9fa;
}
  
nav {
  display: flex;
  gap: 10px;
} */
</style>
