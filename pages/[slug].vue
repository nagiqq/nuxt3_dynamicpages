<template>
<h1>{{ mountain.title }}</h1>
  <p> {{ mountain.description }}</p>
</template>

<script setup>
const route = useRoute()
const { data: mountain } = await useFetch(`https://api.nuxtjs.dev/mountains/${route.params.slug}`)
// TODO: 動態網址為api裡面的slug名稱
</script>

<style scoped>

</style>