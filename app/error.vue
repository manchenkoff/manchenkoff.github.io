<script setup lang="ts">
import type { NuxtError } from '#app'

interface ErrorPageProps {
  error: NuxtError
}

defineProps<ErrorPageProps>()
</script>

<template>
  <UError
    :error="{
      statusMessage: 'Hmmmm...',
      message: 'Looks like you are looking for a wrong stuff',
    }"
  />
</template>
