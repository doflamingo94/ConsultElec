<template>
  <div class="flex flex-col">
    <h1 class="relative title w-full">
      <slot name="title">Titre section 4</slot>
    </h1>
    <div class="image-section w-full flex">
      <div class="image-container">
        <img src="../../assets/css/elec3.jpg" alt="" />
      </div>
      <div class="test">
        <h3 class="w-full font-semibold my-0">
          Une mise en place simple & rapide
        </h3>
        <div class="steps w-full flex flex-col">
          <StepItem
            v-for="(item, ind) in steps"
            :step="item"
            :index="ind + 1"
            :key="item.title + ':' + ind"
          />
        </div>
      </div>
    </div>
  </div>
</template>

<script setup lang="ts">
const imageUrl =
  "/_nuxt/assets/css/elec3.jpg";

const steps = [
  {
    title: "Titre étape",
    description:
      "Lorem ipsum dolor sit amet consectetur adipisicing elit. Laboriosam, temporibus!",
  },
  {
    title: "Titre étape",
    description:
      "Lorem ipsum dolor sit amet consectetur adipisicing elit. Laboriosam, temporibus!",
  },
  {
    title: "Titre étape",
    description:
      "Lorem ipsum dolor sit amet consectetur adipisicing elit. Laboriosam, temporibus!",
  },
];
</script>

<style scoped>
.image-section {
  gap: 2.5rem; /* Adjust the value as needed */
}

/* Alternatively, you can add margin or padding to the individual elements */
.image-container {
  margin-right: 0; /* Adjust the value as needed */
}

@media screen and (max-width: 767px) {
  p {
    text-align: center;
  }
}
</style>
