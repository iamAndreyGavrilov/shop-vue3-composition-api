<template>
  <div class='hero'>
    <HeroInformation
      title='Luxury homeware for people who love timeless design quality'
      description='Shop the new Spring 2022 collection today'
      link='View collection' />
  </div>
</template>

<script setup>
import HeroInformation from '@/components/HeroInformation.vue';

</script>

<style lang='scss' scoped>
.hero {
  background-image: url("public/img/hero.jpg");
  height: 704px;
  background-size: cover;
  display: flex;
  justify-content: flex-end;
  align-items: center;
  padding-right: 60px;
}

</style>