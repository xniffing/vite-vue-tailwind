<template>
  <div class="bg-gray-100 py-5 mx-auto">
    <img class="mx-auto" src="./assets/logo.png" alt="" />
    <p class="text-center text-xl font-bold text-gray-700">{{ title }}</p>
  </div>
  <div class="w-1/2 mx-auto text-center mt-[100px]">
    <button
      @click="buttonClick.click++"
      class="bg-green-700 hover:bg-green-600 text-gray-100 font-bold py-2 px-4 rounded"
    >
      Clicked {{ buttonClick.click }}
    </button>
  </div>
</template>

<script>
import { reactive } from "vue";
export default {
  setup() {
    const buttonClick = reactive({click:0});
    const title = "Vue 3 + Tailwind + Vite";
    return {
      title,
      buttonClick,
    };
  },
};
</script>
<style>
html {
  @apply bg-gray-700;
}
</style>