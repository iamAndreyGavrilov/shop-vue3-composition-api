<template>
  <div class='product'>
    <a href='#' class='product-image'>
      <img :src='img' :alt='title' />
    </a>
    <a href='#' class='product-title'>{{ title }}</a>
    <span class='product-price'>${{ price }}</span>
  </div>
</template>

<script setup>

const props = defineProps({
  title: {
    type: String,
    required: true,
  },
  price: {
    type: Number,
    required: true,
  },
  img: {
    type: String,
    required: true,
  },
});

</script>

<style lang='scss' scoped>
.product {
  display: flex;
  flex-direction: column;
  align-items: center;
  padding: 10px;
  border: 1px solid #eaeaea;
  border-radius: 5px;
  background-color: #fff;
  transition: all 0.3s ease;

  &:hover {
    box-shadow: 0 0 10px rgba(0, 0, 0, 0.5);
  }

  &-image {
    width: 100%;
    height: 100%;
    display: flex;
    justify-content: center;
    align-items: center;

    img {
      max-width: 100%;
      max-height: 100%;
    }
  }

  &-title {
    margin-top: 10px;
    font-size: 1.2rem;
    font-weight: 500;
    color: #333;
    text-decoration: none;
    transition: all 0.3s ease;

    &:hover {
      color: #000;
    }
  }

  &-price {
    margin-top: 10px;
    font-size: 1.2rem;
    font-weight: 500;
    color: #333;
  }
}

</style>