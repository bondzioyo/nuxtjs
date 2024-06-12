<template>
  Test page
  {{ counter }}
  <button type="button" @click.prevent="multiply">addd</button>
</template>
<script setup>
definePageMeta({
  title: "About",
  showInNav: true,
  navPosition: 3,
});
const counter = ref(0);

const multiply = () => {
  counter.value++;
};
</script>
