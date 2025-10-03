<template>
  <section
    class="h-screen flex flex-col justify-center items-center text-center"
    style=""
  >
    <div
      class="absolute top-0 left-0 w-[100%] h-64 bg-gray-900 clip-triangle shadow-triangle"
    ></div>

    <div
      class="absolute bottom-0 right-0 w-[80%] h-64 bg-gray-900 clip-triangle-bottom-right"
    ></div>

   <h1 class="-mt-28 text-[60pt] bg-gradient-to-r from-gray-900 via-gray-800 to-red-600 bg-clip-text text-transparent">{{ "</>" }}</h1>

    <h2 class="text-4xl md:text-6xl font-bold mb-4">
   
      <span
        class="bg-gradient-to-r from-gray-900 via-blue-400 to-red-500 bg-clip-text text-transparent"
        >Artur Cuambe</span
      >
    </h2>
    <p class="text-lg md:text-2xl mb-4">
      Engenheiro de Software | Fullstack Developer
    </p>
    <a
      href="#projects"
      class="bg-blue-950 text-white px-6 py-3 rounded-lg hover:bg-blue-900"
    >
      Ver Portfólio
    </a>
  </section>
</template>
<script setup>
import { CodeBracketIcon } from "@heroicons/vue/24/solid";
</script>
<style>
.clip-triangle {
  clip-path: polygon(0 4%, 90% 0, 0 100%);
  background: linear-gradient(135deg, rgba(0, 0, 0, 0.9), transparent);
}
.clip-triangle-bottom-right {
  clip-path: polygon(100% 0, 100% 90%, 0 90%);
  background: linear-gradient(135deg, rgba(0, 0, 0, 0.9), transparent);
}
.shadow-triangle {
  box-shadow: 5px 5px 60px rgba(201, 25, 25, 0.9);
}
</style>
