<template>
  <div class="card">
    <Carousel :value="products" :responsiveOptions="responsiveOptions">
      <template #item="slotProps">
        <div class=" dark:border-surface-700 rounded mt-4">
          <div class="mb-4">
            <div class="relative mx-auto">
              <img src="https://picsum.photos/200/300" class="w-full h-full rounded" alt="Merchandise"/>
            </div>
          </div>
          <div class="flex justify-between items-center">
            <a :href="slotProps.data.shopifyLink" target="_blank"></a>
          </div>
        </div>
      </template>
    </Carousel>
  </div>
</template>

<script setup>
import { ref } from 'vue';
import { FontAwesomeIcon } from '@fortawesome/vue-fontawesome';
import { faShopify } from '@fortawesome/free-brands-svg-icons';

const products = ref([
  { name: 'Product 1', shopifyLink: 'https://www.shopify.com/product1' },
  { name: 'Product 2', shopifyLink: 'https://www.shopify.com/product2' },
  { name: 'Product 3', shopifyLink: 'https://www.shopify.com/product3' },
]);

const responsiveOptions = ref([
  {
    breakpoint: '1024px',
    numVisible: 1,
    numScroll: 3,
  },
  {
    breakpoint: '768px',
    numVisible: 1,
    numScroll: 3,
  },
  {
    breakpoint: '560px',
    numVisible: 1,
    numScroll: 3,
  },
]);
</script>