<template>
  <div>
    <p>
      These are the params of the URL is: {{ id }} and its details are below--
    </p>
    <p>{{ data.title }}</p>
    <p>${{ data.price }}</p>

    <img :src="data.image" alt="" />
  </div>
</template>

<script setup>
const { id } = useRoute().params;
const uri = "https://fakestoreapi.com/products/" + id;
const { data } = await useFetch(uri);
</script>

<style scoped></style>
