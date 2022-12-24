<template>
  <form class='subscribe-form'>
    <input class='subscribe-form__input' type='email' placeholder='Enter your email address' />
    <UIButton class='subscribe-form__button'>Subscribe</UIButton>
  </form>
</template>

<script setup>
import UIButton from '@/components/UI/Button.vue';
</script>

<style lang='scss' scoped>
.subscribe-form {
  display: flex;
  justify-content: center;
  align-items: center;

  &__input {
    width: 100%;
    max-width: 30rem;
    padding: 1rem 2rem;
    border: none;
    border-radius: 0.5rem 0 0 0.5rem;
    font-size: 1.5rem;
    outline: none;
  }

  &__button {
    padding: 1rem 2rem;
    border: none;
    border-radius: 0 0.5rem 0.5rem 0;
    font-size: 1.5rem;
    background-color: violet;
    color: white;
    cursor: pointer;
    transition: all 0.3s;

    &:hover {
      background-color: darkviolet;
    }
  }
}
</style>