<template>
  <div>
    <NuxtLink :to="`/products/${product.id}`">
      <img :src="product.image" />
      {{ product.price }}
    </NuxtLink>
  </div>
</template>

<script setup>
const { product } = defineProps(["product"]);
</script>

<style scoped>
img {
  height: 200px;
  widows: 200px;
}
</style>
