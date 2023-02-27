<script setup>
import { ref } from "vue";
import CardCategory from "../CardCategory.vue";

const items = ref([
  {
    id: 1,
    title: "RoboCrypto App",
    span: "Mobile Ui Kit",
    img: "categories-1.jpg",
  },
  {
    id: 2,
    title: "Online Doctor Consultation",
    span: "Website Ui Kit",
    img: "categories-2.jpg",
  },
  {
    id: 3,
    title: "Banking Crypto",
    span: "Mobile Ui Kit",
    img: "categories-3.jpg",
  },
]);
</script>

<template>
  <div class="container px-4 mx-auto my-16 md:px-12">
    <h2 class="mb-4 text-xl font-medium md:mb-0 md:text-lg">New Items</h2>
    <div class="flex flex-wrap -mx-1 lg:-mx-4">
      <CardCategory
        v-for="item in items"
        :key="item.id"
        :span="item.span"
        :img="item.img"
        :title="item.title"
      />
    </div>
  </div>
</template>
