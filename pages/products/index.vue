<template>
  <div>
    <div class="getList">
      <div v-for="item in data.slice(0, 10)" :key="item.id">
        <products-card :product="item" />
      </div>
    </div>
  </div>
</template>

<script setup>
const { data } = await useFetch("https://fakestoreapi.com/products");
</script>

<style scoped>
.getList {
  color: blue;
  display: grid;
  grid-template-columns: repeat(5, 1fr);
  gap: 20px;
}
</style>
