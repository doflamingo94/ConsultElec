<template>
  <div class="flex flex-col">
    <h1 class="relative title w-full">
      <slot name="title">Titre section 3</slot>
    </h1>
    <div class="image-section w-full">
      <div class="image-container">
        <img src="../../assets/css/elec2.jpg" alt="" />
      </div>
      <div class="content">
        <p class="text-lg">
          Ce sont tout d’abord
          <span class="font-bold">
            des salariés, des fournisseurs et/ou des cadres d’entreprises avec
            qui nous collaborons
          </span>
          qui sont en déplacement professionnel, ou qui viennent travailler
          quelques jours ou quelques semaines près de chez vous. <br /><br />
          Mais également des salariés qui travaillent durablement dans la région
          et ont besoin d’un logement pour quelques jours ou semaines (période
          d’essai, achat prévu …).
        </p>
      </div>
    </div>
  </div>
</template>

<script setup lang="ts">
const imageUrl =
  "https://www.kan-location.com/wp-content/uploads/2022/03/51617909_l-768x511.jpg";
</script>

<style scoped></style>
