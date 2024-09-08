<script setup lang="ts">
import type { NuxtError } from '#app'

interface ErrorPageProps {
  error: NuxtError
}

defineProps<ErrorPageProps>()
</script>

<template>
  <div class="text-center">
    <h1>{{ error!.statusCode }}</h1>
    <NuxtLink to="/">
      Go back home
    </NuxtLink>
  </div>
</template>
