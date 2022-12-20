<template>
  <div class='container'>
    <Header />
    <Hero />
    <AboutBrand />
    <Products />
    <Ideas />
  </div>
</template>


<script>

import { defineComponent } from 'vue';
import Header from './components/Layout/Header.vue';
import Hero from './components/Hero.vue';
import AboutBrand from './components/AboutBrand.vue';
import Products from './components/Products4Columns.vue';
import Ideas from './components/Ideas.vue';


export default defineComponent({
  components: { Ideas, Products, AboutBrand, Hero, Header },
});


</script>


<style lang='scss'>
@import './styles/global.scss';
</style>
