<style>
img {
  max-width: 10rem;
}
</style>

<template>
  <span>Hello Vite + vite-ssg</span>
  <img :src="dynamicUrl" alt="img1" />
  <img :src="staticUrl" alt="img2" />
</template>

<script setup lang="ts">
const dynamicUrl = new URL('/dip.jpg', import.meta.url).href
const staticUrl = '/dip.jpg'
</script>
