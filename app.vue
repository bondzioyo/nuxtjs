<template>
  <div>
    {{ counter }}
      <button type="button" @click="multiply">addd</button>
    <NuxtWelcome />
  </div>
</template>
<script setup>
const counter = ref(0)

const multiply = () => {
  counter.value++
}

</script>