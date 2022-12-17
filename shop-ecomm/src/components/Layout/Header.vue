<template>
  <header class='header'>
    <div class='header-top'>
      <div class='header-top-search'>
        <img src='/svg/header-search.svg' alt='search'>
      </div>
      <a href='#' class='header-logo'>Avion</a>
      <div class='header-top-right'>
        <div class='header-top-right__cart'>
          <a href='#' >
            <img src='/svg/header-cart.svg' alt='cart'>
          </a>
        </div>
        <div class='header-top-right__avatar'>
        <a href='#' >
          <img src='/svg/header-avatar.svg' alt='avatar'>
        </a>
        </div>
      </div>
    </div>

<!--    <div class='header__bot'>bot</div>-->
  </header>
</template>

<script>
export default {
  name: 'Header',
};
</script>

<style lang='scss' scoped>
.header{
  height: 132px;
  background-color: white;
  &-top{
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    align-items: center;
    height: 70px;
    border-bottom: 1px solid rgba(0, 0, 0, 0.1);
    margin: 0 28px;
    &-right{
      display: flex;
      align-items: center;
      justify-content: flex-end;
      gap: 16px;
      &__cart{
      }
    }
  }
    &-logo{
      text-align: center;
      text-decoration: none;
      color: black;
      font-size: 24px;
      &:hover{
        color: orange;
        text-decoration: underline;
      }
    }
}
</style>