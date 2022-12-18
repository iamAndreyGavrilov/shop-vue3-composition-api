<script>
import { defineComponent } from 'vue';
import Header from './components/Layout/Header.vue';
import Hero from './components/Hero.vue';
import AboutBrand from './components/AboutBrand.vue';

export default defineComponent({
  components: { AboutBrand, Hero, Header },
});

</script>

<template>
  <div class='container'>
    <Header />
    <Hero />
    <AboutBrand />
  </div>
</template>

<style lang='scss'>

.container {
  max-width: 1440px;
  margin: 0 auto;
}

</style>
