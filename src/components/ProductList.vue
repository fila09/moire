<template>
  <ul class="catalog__list">
    <li class="catalog__item" v-for='product in  products' :key="product.id">
      <ProductItem :product="product" />
    </li>
  </ul>
</template>

<script>

import ProductItem from './ProductItem.vue';

export default {
  components: { ProductItem },
  props: ['products'],
};
</script>