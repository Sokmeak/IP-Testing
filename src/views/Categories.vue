<template>
  <div class="container">
    <CardCategory
      v-for="category in categories"
      :key="category.id"
      :fruitName="category.fruitName"
      :item="category.items"
      :image="category.image"
    />
  </div>
</template>

<script>
import { ref } from 'vue';
import CardCategory from '../components/CardCategory.vue';

 export default {
  components: { CardCategory },
  setup() {
    const categories = ref([
      { id: 1, fruitName: 'Peach', items: 14, image: './src/assets/svg/Peach.svg' },
      { id: 2, fruitName: 'Apple', items: 16, image: './src/assets/svg/RedApple.svg' },
      { id: 3, fruitName: 'Snack', items: 17, image: './src/assets/svg/snacks.svg' },
      { id: 4, fruitName: 'Black Plum', items: 27, image: './src/assets/svg/BlackPulm.svg' },
      { id: 5, fruitName: 'Vegetables', items: 21, image: './src/assets/svg/Vegetables.svg' },
      { id: 6, fruitName: 'Headphone', items: 41, image: './src/assets/svg/HeadPhone.svg' },
      { id: 7, fruitName: 'Cake & Milk', items: 89, image: './src/assets/svg/CakeAndMilk.svg' },
      { id: 8, fruitName: 'Orange', items: 13, image: './src/assets/svg/Orange.svg' },
      { id: 9, fruitName: 'Hamburger', items: 23, image: './src/assets/svg/Hamburger.svg' },
      { id: 10, fruitName: 'Kiwi', items: 13, image: './src/assets/svg/Kiwi.svg' },
      { id: 11, fruitName: 'Kiwi', items: 13, image: './src/assets/svg/Kiwi.svg' },
    ]);
    return { categories };
  },
};
</script>
<style>
.container{
  display: flex;
  flex-wrap: wrap;
  gap:12px;
}
</style>
<!-- My file card name CardCategory and big file that contain Card name Category.vue -->