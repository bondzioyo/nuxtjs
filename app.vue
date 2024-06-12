<template>
  <div>
    <NuxtLayout>
      <NuxtPage class="container mx-auto" />
    </NuxtLayout>
  </div>
</template>
<script setup lang="ts">
useHead({
  title: "My amazing site",
  meta: [{ name: "description", content: "My amazing site." }],
});
useSeoMeta({
  title: "My Amazing Siteeee",
  ogTitle: "My Amazing Site",
  description: "This is my amazing site, let me tell you all about it.",
  ogDescription: "This is my amazing site, let me tell you all about it.",
  ogImage: "https://bondzioyo.github.io/assets/angular-BgsP3K5R.webp",
  twitterCard: "summary_large_image",
});
</script>
