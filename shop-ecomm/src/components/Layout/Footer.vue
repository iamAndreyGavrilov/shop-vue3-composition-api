<template>
  <footer class='footer'>
    <div class='footer-content'>
      <div class='footer-top'>
        <div class='footer-menu'>
          <div class='footer-menu-column'>
            <h3 class='footer-menu__title'>Menu</h3>
            <router-link to='/' class='footer-menu__link'>New arrivals</router-link>
            <router-link to='/' class='footer-menu__link'>Best sellers</router-link>
            <router-link to='/' class='footer-menu__link'>Recently viewed</router-link>
            <router-link to='/' class='footer-menu__link'>Popular this week</router-link>
            <router-link to='/' class='footer-menu__link'>All products</router-link>
          </div>
          <div class='footer-menu-column'>
            <h3 class='footer-menu__title'>Categories</h3>
            <router-link to='/' class='footer-menu__link'>Crockery</router-link>
            <router-link to='/' class='footer-menu__link'>Furniture</router-link>
            <router-link to='/' class='footer-menu__link'>Homeware</router-link>
            <router-link to='/' class='footer-menu__link'>Plant pots</router-link>
            <router-link to='/' class='footer-menu__link'>Chairs</router-link>
            <router-link to='/' class='footer-menu__link'>Crockery</router-link>
          </div>
          <div class='footer-menu-column'>
            <h3 class='footer-menu__title'>Our company</h3>
            <router-link to='/' class='footer-menu__link'>About us</router-link>
            <router-link to='/' class='footer-menu__link'>Vacancies</router-link>
            <router-link to='/' class='footer-menu__link'>Contact us</router-link>
            <router-link to='/' class='footer-menu__link'>Privacy</router-link>
            <router-link to='/' class='footer-menu__link'>Returns policy</router-link>
          </div>
        </div>
        <div class='footer-subscribe'>
          <SubscribeForm />
        </div>
      </div>
    </div>

  </footer>
</template>

<script setup>

import SubscribeForm from '@/components/SubscribeForm.vue';
</script>

<style lang='scss' scoped>
.footer {
  //height: 380px;
  background: #2A254B;
  color: white;

  &-content {
    padding: 58px 82px 25px 82px;
  }

  &-top {
    display: grid;
    grid-template-columns: 540px 1fr;
    column-gap: 110px;


  }

  &-menu {
    display: grid;
    grid-template-columns: 1fr 1fr 1fr;

    &__title {

    }

    &__link {
      color: white;
      font-size: 14px;
      line-height: 20px;
      text-decoration: none;
      margin-bottom: 10px;
      display: block;

      &:last-child {
        margin-bottom: 0;
      }

      &:hover {
        text-decoration: underline;
      }

    }
  }

  &-subscribe {
    display: flex;
    align-items: center;
    justify-content: center;
  }
}
</style>