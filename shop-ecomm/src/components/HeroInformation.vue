<template>
  <div :style='{background:backgroundColor}' class='hero-info'>
    <div class='hero-info-text'>
      <p :style='{color:colorTitle}' class='hero-info__title'>{{ title }}</p>
      <span :style='{color:colorDescription}' class='hero-info__description'>{{ description }}</span>
    </div>
    <a href='#' class='hero-info-link'>{{ link }}</a>
  </div>
</template>

<script setup>
const props = defineProps({
  title: {
    type: String,
    required: false,
  },
  description: {
    type: String,
    required: false,
  },
  link: {
    type: String,
    required: false,
  },
  colorTitle: {
    type: String,
    default: '#000',
  },
  colorDescription: {
    type: String,
    default: '#726E8D',
  },
  backgroundColor: {
    type: String,
    default: '#fff',
  },
});

</script>

<style lang='scss' scoped>
.hero {
  &-info {
    background: white;
    max-width: 630px;
    min-height: 444px;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    padding: 50px;
    border-radius: 10px;


    &__title {
      font-size: 32px;
      line-height: 1.5;
      margin: 0 0 20px;
      font-weight: 400;
    }

    &__description {
      font-size: 16px;
    }

    &-link {
      max-width: 170px;
      background: grey;
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
  }
}
</style>