<template>
  <section>
    <h1>PRUEBA</h1>
    <img :src="dogResponse.message" />
  </section>
</template>

<script setup lang="ts">
  const { data: dogResponse } = await useFetch('https://dog.ceo/api/breeds/image/random');
</script>
