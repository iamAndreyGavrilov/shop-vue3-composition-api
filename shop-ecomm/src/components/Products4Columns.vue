<template>
  <div class='products'>
    <div class='products-container'>
      <Product
        v-for='product in products' :key='product.id'
        :img='product.img'
        :title='product.title'
        :price='product.price' />
    </div>
    <a href='#' class='products-link'></a>
  </div>
</template>

<script setup>
import { ref } from 'vue';
import Product from './Product.vue';

const products = ref([
  {
    id: 1,
    title: 'The Dandy chair',
    price: 250,
    img: '/public/img/Product1.png',
  },
  {
    id: 2,
    title: 'Rustic Vase Set',
    price: 155,
    img: '/public/img/Product2.png',
  },
  {
    id: 3,
    title: 'The Silky Vase',
    price: 125,
    img: '/public/img/Product3.png',
  },
  {
    id: 4,
    title: 'The Lucy Lamp',
    price: 399,
    img: '/public/img/Product4.png',
  },
]);
</script>

<style lang='scss' scoped>
.products {
  &-container {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    grid-gap: 10px;
  }
}
</style>