<script setup lang="ts">
const { profiles } = useAppConfig()
</script>

<template>
  <div class="flex gap-4 justify-center">
    <ProfileLink
      v-for="profile in profiles"
      :key="profile.name"
      :profile="profile"
    />
  </div>
</template>

<style scoped></style>
