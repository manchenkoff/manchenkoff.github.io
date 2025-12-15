<script setup lang="ts">
const { seo } = useAppConfig()
</script>

<template>
  <UContainer class="pt-20 sm:pt-28 md:pt-36">
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
  </UContainer>
</template>

<style scoped></style>
