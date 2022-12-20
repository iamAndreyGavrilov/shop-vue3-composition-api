<template>
  <div class='ideas'>
    <HeroInformation
      title='It started with a small idea'
      description='A global brand with local beginnings, our story begain in a small studio in South London in early 2014'
      link='View collection'
      colorTitle='#fff'
      colorDescription='#fff'
      backgroundColor='#2A254B'
    />
    <img class='ideas-img' src='public/img/room.jpg' alt='room'>
  </div>
</template>

<script setup>
import HeroInformation from '@/components/HeroInformation.vue';

</script>

<style lang='scss' scoped>
.ideas {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  padding: 0 80px;
  margin: 60px 0 60px 0;
  column-gap: 16px;

  &-img {
    width: 100%;
    height: 100%;
    object-fit: cover;
    border-radius: 10px;
  }
}
</style>