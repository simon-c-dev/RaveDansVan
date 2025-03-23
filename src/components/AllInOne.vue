<template>
  <div class="py-12 z-10">
    <div class="mx-auto max-w-2xl px-6 lg:max-w-7xl lg:px-8">
      <p class="mx-auto mt-2 max-w-lg text-center text-5xl tracking-tight text-balance text-primary-600 sm:text-7xl" id="rdv">RDV</p>
      <h2 class="text-center text-base/7 text-surface-200 font-semibold">Suis la lumière. Trouve le son.</h2>
      <div class="mt-10 grid gap-4 sm:mt-16 lg:grid-cols-3 lg:grid-rows-2">
        <div class="relative max-lg:order-1 lg:row-span-2 lg:order-1">
          <div class="absolute inset-px rounded-lg bg-surface-900 lg:rounded-l-[2rem]" />
          <div class="relative flex h-full flex-col overflow-hidden rounded-[calc(var(--radius-lg)+1px)] lg:rounded-l-[calc(2rem+1px)]">
            <div class="px-8 pt-4 pb-3 sm:px-10 sm:pt-6 sm:pb-4 text-center flex flex-col h-full">
              <p class="mt-2 text-lg md:text-2xl font-medium tracking-tight text-surface-200">Sur votre agenda</p>
              <div class="mt-4 space-y-4 flex-1 flex flex-col">
                <div class="p-4 bg-surface-700 border-1 border-primary-600 rounded-lg shadow-md flex-1 flex flex-col justify-center">
                  <p class="text-xs text-surface-200">
                    <strong class="font-semibold md:text-lg">2023</strong>
                  </p>
                  <p class="text-xl md:text-3xl font-bold text-surface-200">Jun</p>
                  <p class="text-xl md:text-3xl font-bold text-surface-200">7</p>
                  <hr class="my-4 mx-10 border-surface-600 border-t-2">
                  <p class="text-sm/6 md:text-lg text-surface-200">Red Rocks Amphitheatre</p>
                  <p class="text-sm/6 md:text-lg text-surface-200">Denver, Colorado</p>
                </div>
                <div class="p-4 bg-surface-700 border-1 border-primary-600 rounded-lg shadow-md flex-1 flex flex-col justify-center">
                  <p class="text-xs text-surface-200">
                    <strong class="font-semibold md:text-lg">2023</strong>
                  </p>
                  <p class="text-xl md:text-3xl font-bold text-surface-200">Jul</p>
                  <p class="text-xl md:text-3xl font-bold text-surface-200">15</p>
                  <hr class="my-4 mx-10 border-surface-600 border-t-2">
                  <p class="text-sm/6 md:text-lg text-surface-200">Madison Square Garden</p>
                  <p class="text-sm/6 md:text-lg text-surface-200">New York, New York</p>
                </div>
              </div>
            </div>
          </div>
          <div class="pointer-events-none absolute inset-px rounded-lg ring-1 shadow-sm ring-black/5 lg:rounded-l-[2rem]" />
        </div>
        <div class="relative max-lg:order-2 lg:order-2">
        <div class="absolute inset-px rounded-lg bg-surface-900" />
          <div class="relative text-center flex h-full flex-col overflow-hidden rounded-[calc(var(--radius-lg)+1px)] max-lg:rounded-t-[calc(2rem+1px)]">
            <a href="https://www.instagram.com" target="_blank" class="px-8 pt-4 sm:px-10 sm:pt-6 flex flex-col h-full">
              <p class="mt-2 text-lg md:text-2xl font-medium tracking-tight text-surface-200 max-lg:text-center">Suis-nous sur Instagram</p>
              <p class="mt-2 max-w-lg text-sm sm:text-base lg:text-lg text-surface-200 max-lg:text-center">Actus, exclus, et événements à ne pas rater !</p>
              <div class="flex flex-1 items-center justify-center px-8 max-lg:pt-10 max-lg:pb-12 sm:px-10 lg:pb-2">
                <font-awesome-icon :icon="['fab', 'instagram']" class="text-7xl text-primary-600 hover:text-surface-200" />
              </div>
            </a>
          </div>
          <div class="pointer-events-none absolute inset-px rounded-lg ring-1 shadow-sm ring-black/5 max-lg:rounded-t-[2rem]" />
        </div>
        <div class="relative max-lg:row-start-3 lg:col-start-2 lg:row-start-2 lg:order-3 order-3">
          <div class="absolute inset-px rounded-lg bg-surface-900" />
          <div class="relative text-center flex h-full flex-col overflow-hidden rounded-[calc(var(--radius-lg)+1px)]">
            <div class="px-8 pt-4 sm:px-10 sm:pt-6">
              <p class="mt-2 text-lg md:text-2xl font-medium tracking-tight text-surface-200 max-lg:text-center">RDV Radio Patreon</p>
              <p class="mt-2 max-w-lg text-sm sm:text-base lg:text-lg text-surface-100 max-lg:text-center">Plonge dans le son ! Abonne-toi à RDV Radio pour des sets DJ exclusifs.</p>
            </div>
            <div class="flex flex-1 items-center justify-center max-lg:py-6 lg:pb-2">
              <font-awesome-icon :icon="['fab', 'patreon']" class="text-7xl text-primary-600 hover:text-surface-200" />
            </div>
          </div>
          <div class="pointer-events-none absolute inset-px rounded-lg ring-1 shadow-sm ring-black/5" />
        </div>
        <div class="relative lg:row-span-2 lg:order-4 order-4">
          <div class="absolute inset-px rounded-lg bg-surface-900 max-lg:rounded-b-[2rem] lg:rounded-r-[2rem]" />
          <div class="relative text-center flex h-full flex-col overflow-hidden rounded-[calc(var(--radius-lg)+1px)] max-lg:rounded-b-[calc(2rem+1px)] lg:rounded-r-[calc(2rem+1px)]">
            <a href="https://www.shopify.com" target="_blank" class="pb-3 sm:pb-4 px-8 pt-4 sm:px-10 sm:pt-6 flex flex-col h-full shopify-image">
              <p class="mt-2 text-lg md:text-2xl font-medium tracking-tight text-surface-200 max-lg:text-center">Boutique RDV</p>
              <p class="mt-2 max-w-lg text-sm sm:text-base lg:text-lg text-surface-200 max-lg:text-center">La musique se porte aussi ! Explore notre collection sur Shopify</p>
              <carousel-tee/>
            </a>
          </div>
          <div class="pointer-events-none absolute inset-px rounded-lg ring-1 shadow-sm ring-black/5 max-lg:rounded-b-[2rem] lg:rounded-r-[2rem]" />
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
import { ref } from 'vue';
import { FontAwesomeIcon } from '@fortawesome/vue-fontawesome';
import { faInstagram, faShopify, faPatreon } from '@fortawesome/free-brands-svg-icons';
import CarouselTee from "./sub/carouselTee.vue";

const links = ref([
  { name: 'Instagram', href: 'https://www.instagram.com', icon: faInstagram },
  { name: 'Shopify', href: 'https://www.shopify.com', icon: faShopify },
  { name: 'Patreon', href: 'https://www.patreon.com', icon: faPatreon },
]);
</script>

<style scoped>
@media (min-width: 650px) {
  .shopify-image {
    max-width: 400px; /* Ajuste la taille maximale de l'image */
    height: auto; /* Garde le ratio de l'image */
    margin: 0 auto; /* Centre l'image */
  }

  .p-carousel-prev,
  .p-carousel-next {
    display: none !important;
  }

}
</style>