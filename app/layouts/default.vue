<script setup lang="ts">
useHead({
  htmlAttrs: {
    lang: 'en',
  },
  meta: [
    { charset: 'utf-8' },
    { name: 'viewport', content: 'width=device-width, initial-scale=1' },
  ],
  link: [
    {
      rel: 'icon',
      href: '/favicon.ico',
    },
    {
      rel: 'shortcut icon',
      href: '/favicon.ico',
    },
    {
      rel: 'apple-touch-icon',
      href: '/favicon.ico',
    },
  ],
})
</script>

<template>
  <ImageBackground />

  <UMain class="flex flex-col gap-4 justify-center items-center">
    <UContainer>
      <slot />
    </UContainer>

    <UColorModeSwitch />
  </UMain>
</template>

<style scoped></style>
