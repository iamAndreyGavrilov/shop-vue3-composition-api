<template>
  <div class='hero'>
    <HeroInformation
      title='Luxury homeware for people who love timeless design quality'
      description='Shop the new Spring 2022 collection today'
      link='View collection' />
  </div>
</template>

<script setup>
import HeroInformation from './HeroInformation.vue';

</script>

<style lang='scss' scoped>
.hero {
  background: url('https://images.pexels.com/photos/1571460/pexels-photo-1571460.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=2');
  height: 704px;
  background-size: cover;
  display: flex;
  justify-content: flex-end;
  align-items: center;
  padding-right: 60px;
}

</style>