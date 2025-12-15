<script setup lang="ts">
const { seo } = useAppConfig()

useSeoMeta({
  title: seo.title,
  description: seo.description,

  ogTitle: seo.title,
  ogDescription: seo.description,
  ogImage: seo.image,
  ogUrl: '/',

  twitterTitle: seo.title,
  twitterDescription: seo.description,
  twitterImage: seo.image,
  twitterCard: 'summary',
})
</script>

<template>
  <ProfileCard />
</template>

<style scoped></style>
