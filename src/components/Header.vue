<template>
  <nav class="bg-white text-gray-900 p-4 flex justify-between items-center  shadow-md fixed w-full z-50 ">
    <div class="text-xl font-bold">Artur Cuambe</div>
    
    <!-- Botão Hamburger (mobile) -->
    <button 
      @click="toggleMenu" 
      class="md:hidden focus:outline-none"
    >
      <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6" fill="none"
           viewBox="0 0 24 24" stroke="currentColor">
        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
              d="M4 6h16M4 12h16M4 18h16"/>
      </svg>
    </button>

    <!-- Menu desktop -->
    <ul class="hidden md:flex space-x-6">
      <li><a href="#about" class="hover:text-gray-400">Sobre</a></li>
      <!-- <li><a href="#formacao" class="hover:text-gray-400">Formação</a></li> -->
      <li><a href="#projects" class="hover:text-gray-400">Portfólio</a></li>
      <li><a href="#contact" class="hover:text-gray-400">Contato</a></li>
    </ul>

    <!-- Menu mobile -->
    <ul v-if="isOpen" class="absolute top-16 left-0 text-gray-900 w-full -mt-1 bg-gray-50 flex flex-col items-baseline  space-y-4 py-4 md:hidden">
      <li><a @click="closeMenu" href="#about" class="hover:text-gray-900 mx-4">Sobre</a></li>
      <!-- <li><a @click="closeMenu" href="#formacao" class="hover:text-gray-100 mx-4">Formação</a></li> -->
      <li><a @click="closeMenu" href="#projects" class="hover:text-gray-100 mx-4">Portfólio</a></li>
      <li><a @click="closeMenu" href="#contact" class="hover:text-gray-100 mx-3">Contato</a></li>
    </ul>
  </nav>
</template>

<script setup>
import { ref } from 'vue'

const isOpen = ref(false)

function toggleMenu() {
  isOpen.value = !isOpen.value
}

function closeMenu() {
  isOpen.value = false
}
</script>
