<template>
  <div class='subscribe'>
    <div class='subscribe__content'>
      <h2 class='subscribe__title'>Subscribe to our newsletter</h2>
      <p class='subscribe__text'>Subscribe to our newsletter and get 10% off your first purchase</p>
      <SubscribeForm />
    </div>
  </div>
</template>

<script setup>
import SubscribeForm from '@/components/SubscribeForm.vue';

</script>

<style lang='scss' scoped>
.subscribe {
  height: 440px;
  background-image: url("public/img/subscribe.jpg");
  background-size: cover;
  background-position: center;
  background-repeat: no-repeat;
  padding: 5rem 0;
  text-align: center;
  color: white;

  &__content {
    max-width: 50rem;
    margin: 0 auto;
  }

  &__title {
    font-size: 2.5rem;
    font-weight: 700;
    margin-bottom: 1rem;
  }

  &__text {
    font-size: 1.5rem;
    margin-bottom: 2rem;
  }
}

</style>