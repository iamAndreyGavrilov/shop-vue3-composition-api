<template>
  <div :style='{background:backgroundColor}' class='hero-info'>
    <div class='hero-info-text'>
      <p :style='{color:colorTitle}' class='hero-info__title'>{{ title }}</p>
      <span :style='{color:colorDescription}' class='hero-info__description'>{{ description }}</span>
    </div>
    <!--    <a href='#' class='hero-info-link'>{{ link }}</a>-->
    <UIButton type='link' background='#4E4D93' to='/'>
      View collection
    </UIButton>
  </div>
</template>

<script setup>
import UIButton from '@/components/UI/Button.vue';

const props = defineProps({
  title: {
    type: String,
    required: false,
  },
  description: {
    type: String,
    required: false,
  },
  link: {
    type: String,
    required: false,
  },
  colorTitle: {
    type: String,
    default: 'black',
  },
  colorDescription: {
    type: String,
    default: 'purple',
  },
  backgroundColor: {
    type: String,
    default: 'white',
  },
});

</script>

<style lang='scss' scoped>
.hero {
  &-info {
    background: var(--color-white);
    max-width: 630px;
    min-height: 444px;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    padding: 50px;
    border-radius: 10px;


    &__title {
      font-size: 32px;
      line-height: 1.5;
      margin: 0 0 20px;
      font-weight: 400;
    }

    &__description {
      font-size: 16px;
    }
  }
}
</style>