<template>
  <button v-if="type === 'button'" class='btn' :style='{backgroundColor: background}'>
    <slot></slot>
  </button>
  <router-link :to='to' v-else class='btn' :style='{backgroundColor: background}'>
    <slot></slot>
  </router-link>

</template>

<script setup>
const props = defineProps({
  background: {
    type: String,
  },
  type: {
    type: String,
    default: 'button',
  },
  to: {
    type: String,
  },
});

</script>

<style lang='scss' scoped>


.btn {
  display: block;
  max-width: 170px;
  background: var(--color-violet);
  color: var(--color-white);
  padding: 10px 20px;
  border-radius: 5px;
  text-decoration: none;
  transition: all 0.3s ease-in-out;
  text-align: center;


  &:hover {
    background: var(--color-white);
    color: var(--color-orange);
    cursor: pointer;
  }
}
</style>