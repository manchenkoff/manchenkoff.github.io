<script setup lang="ts">
const appConfig = useAppConfig()

useHead({
  titleTemplate: pageTitle => pageTitle ? `${pageTitle} - ${appConfig.title}` : `${appConfig.title}`,
})

const colorMode = useColorMode()

colorMode.preference = 'light'
</script>

<template>
  <NuxtLoadingIndicator />
  <NuxtLayout>
    <UApp>
      <NuxtPage />
    </UApp>
  </NuxtLayout>
</template>

<style scoped></style>
