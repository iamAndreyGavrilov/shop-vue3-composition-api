<template>
  <div class='container'>
    <Header />
    <Hero />
    <AboutBrand />
    <Products />
  </div>
</template>


<script>

import { defineComponent } from 'vue';
import Header from './components/Layout/Header.vue';
import Hero from './components/Hero.vue';
import AboutBrand from './components/AboutBrand.vue';
import Products from './components/Products4Columns.vue';


export default defineComponent({
  components: { Products, AboutBrand, Hero, Header },
});


</script>


<style lang='scss'>

.container {
  max-width: 1440px;
  margin: 0 auto;
}

</style>
