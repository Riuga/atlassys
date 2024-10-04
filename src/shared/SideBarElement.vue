<template>
  <li>
    <img :src="getURL()" alt="">
    <p>{{ title }}</p>
  </li>
</template>

<script setup>
const props = defineProps({
  title: String,
  img: String
})

const getURL = () => {
  return new URL(`../assets/sidebar/${img}`, import.meta.url)
}
</script>

<style></style>