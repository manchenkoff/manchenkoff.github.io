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
  <UMain>
    <ImageBackground />

    <slot />

    <div class="flex absolute bottom-4 w-full justify-center md:fixed md:right-4 md:w-fit">
      <UColorModeSwitch />
    </div>
  </UMain>
</template>

<style scoped></style>
