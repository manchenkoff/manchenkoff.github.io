<script setup lang="ts">
const appConfig = useAppConfig()

useHead({
  titleTemplate: pageTitle => pageTitle ? `${pageTitle} - ${appConfig.title}` : appConfig.title,
})
</script>

<template>
  <NuxtLoadingIndicator />
  <NuxtLayout>
    <NuxtPage />
  </NuxtLayout>
</template>

<style scoped></style>
