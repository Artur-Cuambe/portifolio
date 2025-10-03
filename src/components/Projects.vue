<template>
  <section id="projects" class="py-20 bg-gray-50" ref="projectsSection">
    <h3 class="text-3xl font-bold mb-10 text-center">Projetos</h3>
    <div class="grid md:grid-cols-2 lg:grid-cols-3 gap-8 mx-8">
      <div 
        v-for="(project, index) in projects" 
        :key="index"
        class="bg-white shadow-md rounded-lg p-6 transform opacity-0 translate-y-6 transition-all duration-700 ease-out"
        :class="{ 'opacity-100 translate-y-0': project.visible }"
      >
        <h4 class="text-xl font-semibold mb-2">{{ project.name }}</h4>
        <p class="text-gray-600">{{ project.description }}</p>
      </div>
    </div>
  </section>
</template>

<script setup>
import { ref, onMounted } from 'vue'

const projectsSection = ref(null)

const projects = ref([
  { name: 'Agendamento de Posts', description: 'Aplicação para agendar posts em redes sociais (Instagram, Facebook, Twitter) com NestJS, Prisma e cron jobs.', visible: false },
  { name: 'Gestão de Encomendas', description: 'Sistema completo para gestão de encomendas com Prisma, Vue.js e integração backend NestJS.', visible: false },
  { name: 'Outro Projeto Exemplo', description: 'Descrição do projeto exemplo para animação.', visible: false }
])

onMounted(() => {
  const observer = new IntersectionObserver(
    (entries) => {
      if (entries[0].isIntersecting) {
        // Reset e animação escalonada
        projects.value.forEach((p) => (p.visible = false))
        projects.value.forEach((p, index) => {
          setTimeout(() => {
            p.visible = true
          }, index * 150)
        })
      }
    },
    { threshold: 0.3 }
  )

  if (projectsSection.value) {
    observer.observe(projectsSection.value)
  }
})
</script>
