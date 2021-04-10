<template>
<div class="bg-indigo-700 py-5 mx-auto">
    <p class="text-center text-xl font-bold text-gray-100">{{title}}</p>
</div>
<div class="w-1/2 mx-auto text-center mt-[100px]">
<button @click="buttonClick++" class="bg-blue-500 hover:bg-blue-700 text-white font-bold py-2 px-4 rounded">
  Clicked {{buttonClick}}
</button>
</div>
</template>

<script>
import {ref} from 'vue'
export default {
  setup() {
    const buttonClick = ref(0)
    const title = 'Vue 3 + Tailwind + Vite'
    return {
      title,
      buttonClick
    }
  }
}
</script>
<style>
html {
    @apply bg-gray-700
}
</style>