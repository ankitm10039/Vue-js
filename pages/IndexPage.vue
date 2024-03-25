<template>
  <q-page class="p-6">
    <div
      class="grid grid-cols-1 sm:grid-cols-2 md:grid-cols-3 lg:grid-cols-3 xl:grid-cols-4 gap-4"
    >
      <MyCard
        v-for="item in [...list, ...list]"
        :key="item.title"
        v-bind="item"
      />
    </div>
  </q-page>
</template>

<script setup>
import MyCard from "src/components/MyCard.vue";
import { ref } from "vue";

defineOptions({
  name: "IndexPage",
});

const list = ref([
  {
    imgSrc: "https://cdn.quasar.dev/img/mountains.jpg",
    title: "First Card",
    description: "This is the description for the first card.",
  },
  {
    imgSrc: "https://cdn.quasar.dev/img/mountains.jpg",
    title: "Second Card",
    description: "This is the description for the second card.",
  },
  {
    imgSrc: "https://cdn.quasar.dev/img/mountains.jpg",
    title: "Third Card",
    description: "This is the description for the third card.",
  },
  {
    imgSrc: "https://cdn.quasar.dev/img/mountains.jpg",
    title: "Fourth Card",
    description: "This is the description for the fourth card.",
  },
  {
    imgSrc: "https://cdn.quasar.dev/img/mountains.jpg",
    title: "Fifth Card",
    description: "This is the description for the fifth card.",
  },
  {
    imgSrc: "https://cdn.quasar.dev/img/mountains.jpg",
    title: "Sixth Card",
    description: "This is the description for the sixth card.",
  },
  {
    imgSrc: "https://cdn.quasar.dev/img/mountains.jpg",
    title: "Seventh Card",
    description: "This is the description for the seventh card.",
  },
  {
    imgSrc: "https://cdn.quasar.dev/img/mountains.jpg",
    title: "Eighth Card",
    description: "This is the description for the eighth card.",
  },
  {
    imgSrc: "https://cdn.quasar.dev/img/mountains.jpg",
    title: "Ninth Card",
    description: "This is the description for the ninth card.",
  },
  {
    imgSrc: "https://cdn.quasar.dev/img/mountains.jpg",
    title: "Tenth Card",
    description: "This is the description for the tenth card.",
  },
]);
</script>
