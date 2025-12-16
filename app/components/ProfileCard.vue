<script setup lang="ts">
const { seo } = useAppConfig()
</script>

<template>
  <UPageCard
    title="Artem Manchenkov"
    description="software engineer | open-source contributor | public speaker"
    variant="soft"
    spotlight
    :ui="{ root: 'sm:max-w-md mx-auto', wrapper: 'items-center text-center' }"
  >
    <template #header>
      <img
        src="~/assets/images/avatar.png"
        width="200"
        :alt="seo.title"
        class="rounded-full"
      >
    </template>

    <ProfileLinkList />
  </UPageCard>
</template>

<style scoped></style>
