<template>
  <header class="h-[60px] flex items-center bg-yellow-300">
    <nav class="flex gap-[30px] container mx-auto">
      <NuxtLink
        v-for="route in existingRoutes"
        class="hover:text-purple-700"
        :to="route"
        >{{ route.meta.title }}</NuxtLink
      >
    </nav>
  </header>
</template>
<script setup>
const existingRoutes = useRouter()
  .getRoutes()
  .filter((el) => el.meta.showInNav)
  .sort((a, b) => Number(a.meta.navPosition) - Number(b.meta.navPosition));
</script>
