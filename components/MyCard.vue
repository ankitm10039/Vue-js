<template>
  <q-card class="my-card">
    <img :src="imgSrc" />

    <q-card-section>
      <div class="text-h6">{{ title }}</div>
      <div class="text-subtitle2">by John Doe</div>
    </q-card-section>

    <q-card-section class="q-pt-none">
      {{ description }}
    </q-card-section>
  </q-card>
</template>

<script setup>
const props = defineProps({
  description: String,
  imgSrc: String,
  title: String,
});
</script>
