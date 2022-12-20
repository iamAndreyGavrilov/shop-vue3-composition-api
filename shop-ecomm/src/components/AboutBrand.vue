<template>
  <div class='about-brand'>
    <p class='about-brand__title'>What makes our brand different</p>
    <div class='about-brand-elements'>
      <div class='about-brand-element' v-for='(element,i) in aboutBrands' key='i'>
        <img :src='element.img' :alt='element.title' class='about-brand-element__img'>
        <h4 class='about-brand-element__title'>{{ element.title }}</h4>
        <span
          class='about-brand-element__description'>{{ element.description }}</span>
      </div>
    </div>
  </div>
</template>

<script setup>
import { ref } from 'vue';

const aboutBrands = [
  {
    img: 'public/svg/about-brand-delivery.svg',
    title: 'Next day as standard',
    description: 'Order before 3pm and get your order the next day as standard',
  },
  {
    img: 'public/svg/about-brand-outline.svg',
    title: 'Made by true artisans',
    description: 'Handmade crafted goods made with real passion and craftmanship',
  },
  {
    img: 'public/svg/about-brand-purchase.svg',
    title: 'Unbeatable prices',
    description: 'For our materials and quality you won’t find better prices anywhere',
  },
  {
    img: 'public/svg/about-brand-sprout.svg',
    title: 'Recycled packaging',
    description: 'We use 100% recycled to ensure our footprint is more manageable',
  },
];

</script>

<style lang='scss' scoped>
.about-brand {
  padding: 50px 0;

  &__title {
    font-size: 24px;
    color: var(--color-black);
    line-height: 1.5;
    margin: 0 0 20px;
    text-align: center;
  }

  &-elements {
    display: grid;
    grid-template-columns: repeat(4, 210px);
    justify-content: space-between;
    grid-gap: 20px;
    padding: 0 20px;
  }

  &-element {
    &__img {
      margin-bottom: 10px;
    }

    &__title {
      font-size: 20px;
      color: var(--color-black);
      line-height: 1.5;
      margin: 0 0 10px;
    }

    &__description {
      font-size: 14px;
      color: var(--color-black);
      line-height: 1.5;
      margin: 0;
    }
  }
}
</style>