<template>
  <header class='header'>
    <div class='header-top'>
      <div class='header-top-search'>
        <img src='/svg/header-search.svg' alt='search'>
      </div>
      <a href='#' class='header-logo'>Avion</a>
      <div class='header-top-right'>
        <div class='header-top-right__cart'>
          <a href='#'>
            <img src='/svg/header-cart.svg' alt='cart'>
          </a>
        </div>
        <div class='header-top-right__avatar'>
          <a href='#'>
            <img src='/svg/header-avatar.svg' alt='avatar'>
          </a>
        </div>
      </div>
    </div>

    <div class='header-menu'>
      <a class='header-menu__link'
         :href='element.path' v-for='(element, i) in menu' :key='i'>
        {{ element.name }}
      </a>
    </div>
  </header>
</template>

<script setup>
import { ref } from 'vue';

const menu = [
  {
    name: 'Plant pots',
    path: '/plant',
  },
  {
    name: 'Ceramics',
    path: '/ceramics',
  },
  {
    name: 'Tables',
    path: '/tables',
  },
  {
    name: 'Plant pots',
    path: '/plant',
  },
  {
    name: 'Chairs',
    path: '/chairs',
  },
  {
    name: 'Crockery',
    path: '/crockery',
  },
  {
    name: 'Tableware',
    path: '/tableware',
  },
  {
    name: 'Cutlery',
    path: '/cutlery',
  },
];

</script>

<style lang='scss' scoped>
.header {
  height: 132px;
  background-color: var(--color-white);

  &-top {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    align-items: center;
    height: 70px;
    border-bottom: 1px solid rgba(0, 0, 0, 0.1);
    margin: 0 28px;

    &-right {
      display: flex;
      align-items: center;
      justify-content: flex-end;
      gap: 16px;

      &__cart {
      }
    }
  }

  &-logo {
    text-align: center;
    text-decoration: none;
    color: var(--color-black);
    font-size: 24px;

    &:hover {
      color: var(--color-orange);
      text-decoration: underline;
    }
  }

  &-menu {
    height: 62px;
    display: flex;
    align-items: center;
    justify-content: center;
    gap: 44px;

    &__link {
      text-decoration: none;
      color: var(--color-purple);

      &:hover {
        color: var(--color-orange);
        text-decoration: underline;
      }
    }
  }
}
</style>