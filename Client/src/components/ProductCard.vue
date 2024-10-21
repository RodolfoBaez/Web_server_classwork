<script setup lang="ts">
import type { Product } from '@/models/products'

defineProps<{
  product: Product
}>()
</script>

<template>
  <div class="box">
    <div class="box-image">
      <img :src="product.thumbnail" alt="product.name" />
    </div>
    <div class="box-content">
      <h3>{{ product.title }}</h3>
      <i>{{ product.brand }}</i>
      <p>{{ product.description }}</p>
      <p class="price">${{ product.price }}</p>
      <button class="button is-sucess">add to cart</button>
    </div>
  </div>
</template>

<style scoped>
h3 {
  font-weight: bold;
}
.price {
  font-size: 1.5rem;
  font-weight: bold;
  float: right;
}
</style>
