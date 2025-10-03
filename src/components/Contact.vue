<template>
  <section id="contact" class="py-20 bg-gray-100">
    <h3 class="text-3xl font-bold mb-10 text-center">Contato</h3>
    <div class="container mx-auto grid md:grid-cols-2 gap-12">
      
      <!-- Lado esquerdo: informações de contato com ícones -->
      <div class="flex flex-col justify-center space-y-6 text-gray-700">
        <div class="flex items-center space-x-3">
          <EnvelopeIcon class="h-6 w-6 text-blue-600"/>
          <span>logan.cuambe@email.com</span>
        </div>
        <div class="flex items-center space-x-3">
          <PhoneIcon class="h-6 w-6 text-blue-600"/>
          <span>+258 84 954 3940</span>
        </div>
        <div class="flex items-center space-x-3">
          <MapPinIcon class="h-6 w-6 text-blue-600"/>
          <span>Maputo, Moçambique</span>
        </div>
        <p class="mt-4">Sinta-se à vontade para entrar em contato! Vou responder o mais rápido possível.</p>
      </div>

      <!-- Lado direito: formulário -->
      <div>
        <form class="space-y-4">
          <input type="text" placeholder="Seu Nome" class="w-full border p-3 rounded focus:outline-none focus:ring-2 focus:ring-blue-600" />
          <input type="email" placeholder="Seu Email" class="w-full border p-3 rounded focus:outline-none focus:ring-2 focus:ring-blue-600" />
          <textarea placeholder="Sua Mensagem" class="w-full border p-3 rounded h-32 focus:outline-none focus:ring-2 focus:ring-blue-600"></textarea>
          <button type="submit" class="w-full bg-blue-600 text-white py-3 rounded hover:bg-blue-700 transition-colors duration-300">
            Enviar
          </button>
        </form>
      </div>

    </div>
  </section>
</template>

<script setup>
import { EnvelopeIcon, PhoneIcon, MapPinIcon } from '@heroicons/vue/24/solid'
</script>
