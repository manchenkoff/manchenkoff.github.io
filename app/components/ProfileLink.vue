<script setup lang="ts">
type Profile = {
  name: string
  url: string
}

type Props = {
  profile: Profile
}

const props = defineProps<Props>()

const iconName = `i-simple-icons-${props.profile.name}`
</script>

<template>
  <UButton
    :icon="iconName"
    variant="ghost"
    :to="props.profile.url"
    target="_blank"
  />
</template>

<style scoped></style>
