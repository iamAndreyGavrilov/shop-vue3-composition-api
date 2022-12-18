<template>
  <div class='hero'>
    <div class='hero-info'>
      <div class='hero-info-text'>
        <p class='hero-info__title'>Luxury homeware for people who love timeless design quality</p>
        <span class='hero-info__description'>Shop the new Spring 2022 collection today</span>
      </div>
      <a href='#' class='hero-info-link'>View collection</a>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Hero',
};
</script>

<style lang='scss' scoped>
.hero {
  background: url('https://images.pexels.com/photos/1571460/pexels-photo-1571460.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=2');
  height: 704px;
  background-size: cover;
  display: flex;
  justify-content: flex-end;
  align-items: center;
  padding-right: 60px;

  &-info {
    background: white;
    max-width: 630px;
    height: 444px;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    padding: 50px;
    border-radius: 10px;

    &-link {
      max-width: 170px;
      background: #000;
      color: #fff;
      padding: 10px 20px;
      border-radius: 5px;
      text-decoration: none;
      transition: all 0.3s ease-in-out;
      text-align: center;

      &:hover {
        background: #fff;
        color: orange;
      }
    }

    &__title {
      font-size: 32px;
      color: #000;
      line-height: 1.5;
      margin: 0 0 20px;
      font-weight: 400;
    }

    &__description {
      font-size: 16px;
      color: #726E8D;
    }
  }
}

</style>