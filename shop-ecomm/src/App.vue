<script>
import { defineComponent } from 'vue';
import Header from './components/Layout/Header.vue';

export default defineComponent({
  components: { Header },
});
</script>

<template>
  <div class='container'>
    <Header />

  </div>
</template>

<style lang="scss">

.container {
  max-width: 1440px;
  margin: 0 auto;
}

</style>
