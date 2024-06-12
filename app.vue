<template>
  <div>
    <NuxtLayout>
      <NuxtPage class="container mx-auto" />
    </NuxtLayout>
  </div>
</template>
<script setup lang="ts">
useHead({
  title: "My amazing siteedasdsee",
  meta: [{ name: "description", content: "My amazing site." }],
  bodyAttrs: {
    class: "test",
  },
  script: [{ innerHTML: "console.log('Hello world')" }],
});
useSeoMeta({
  title: "My Amazing Siteeee",
  ogTitle: "My Amazing Site",
  description: "This is my amazing site, let me tell you all about it.",
  ogDescription: "This is my amazing site, let me tell you all about it.",
  ogImage: "https://example.com/image.png",
  twitterCard: "summary_large_image",
});
</script>
