<script setup>
import { ref } from "vue";
import CardCategory from "../CardCategory.vue";

const categories = ref([
  {
    id: 1,
    title: "Website Ui Kit",
    count: 731,
    img: "categories-1.jpg",
  },
  {
    id: 2,
    title: "Fonts",
    count: 657,
    img: "categories-2.jpg",
  },
  {
    id: 3,
    title: "Icon Set",
    count: 83.599,
    img: "categories-3.jpg",
  },
  {
    id: 4,
    title: "Website Ui Kit",
    count: 4.5,
    img: "categories-4.jpg",
  },
]);
</script>

<template>
  <div class="container px-4 mx-auto my-16 md:px-12">
    <h2 class="mb-4 text-xl font-medium md:mb-0 md:text-lg">Top Categories</h2>
    <div class="flex flex-wrap -mx-1 lg:-mx-4">
      <CardCategory
        v-for="category in categories"
        :key="category.id"
        :title="category.title"
        :count="category.count"
        :img="category.img"
      />
    </div>
  </div>
</template>
