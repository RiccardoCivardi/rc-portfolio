<script setup lang="ts">
import { useHead } from '@unhead/vue'

useHead({
  htmlAttrs: { lang: 'it' },
  titleTemplate: (title) =>
    title ? `${title} | Riccardo Civardi` : 'Riccardo Civardi — Frontend Developer',
})
</script>

<template>
  <h1>Portfolio</h1>

  Visit <a href="https://vuejs.org/" target="_blank" rel="noopener">vuejs.org</a> to read the
  documentation
  <RouterLink to="/about">About</RouterLink>
  <RouterLink to="/">Home</RouterLink>
  <RouterView />
</template>

<style scoped></style>
