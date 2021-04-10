<template>
<div class="bg-indigo-700 py-5 mx-auto">
    <p class="text-center text-xl font-bold text-gray-100">{{title}}</p>
</div>
<div class="">
    <button class="bg-blue-500 hover:bg-blue-700 text-white font-bold py-2 px-4 rounded">
  Button
</button>
</div>
</template>

<script>
export default {
  setup() {
    const title = 'Vue 3 + Tailwind + Vite'
    return {
      title
    }
  }
}
</script>
<style>
html {
    @apply bg-gray-700
}
</style>