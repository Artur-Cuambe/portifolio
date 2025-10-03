<template>
  <section id="about" class="py-20 bg-white -mt-28">
    <h3 class="text-3xl font-bold mb-12 text-center">Sobre Mim</h3>
    <div class=" mx-8 md:flex md:items-center md:space-x-12">
      
      <!-- Lado esquerdo: foto ou avatar -->
      <div class="md:w-1/3 mb-8 md:mb-0 flex justify-center">
        <img src="/src/assets/images/eu.jpg" alt="Logan Cuambe" class="rounded-full shadow-lg w-64 h-64 object-cover"/>
      </div>

      <!-- Lado direito: texto + skills -->
      <div class="md:w-2/3 text-gray-700 space-y-6">
        <p class="text-lg leading-relaxed">
          Sou licenciado em Informática com minor em Engenharia de Desenvolvimento de Sistemas pela Universidade Pedagógica de Maputo (UPM). 
          Atuo como Engenheiro de Software com experiência em NestJS, Node.js, GraphQL, Prisma e Vue.js, criando soluções web escaláveis e integrando APIs modernas.
        </p>

        <div>
          <h4 class="text-xl font-semibold mb-4">Minhas principais habilidades:</h4>
          <ul class="space-y-2">
            <li class="flex items-center">
              <CheckIcon class="h-5 w-5 text-blue-600 mr-2"/>
              Desenvolvimento Frontend: Vue.js, TailwindCSS
            </li>
            <li class="flex items-center">
              <CheckIcon class="h-5 w-5 text-blue-600 mr-2"/>
              Backend: Node.js, NestJS, GraphQL, Prisma
            </li>
            <li class="flex items-center">
              <CheckIcon class="h-5 w-5 text-blue-600 mr-2"/>
              Integração de APIs e automação de processos
            </li>
          </ul>
        </div>

      </div>

    </div>
  </section>
</template>

<script setup>
import { CheckIcon } from '@heroicons/vue/24/solid'
</script>
