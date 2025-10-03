<template>
  <div class="font-sans bg-gray-100 text-gray-900">
    <Header />
    <main class="container mx-auto px-6 pt-20">
      <Hero />
      <About />
      <Projects />
      <Contact />
    </main>
    <Footer />
  </div>
</template>

<script setup>
import Header from "./components/Header.vue";
import Hero from "./components/Hero.vue";
import About from "./components/About.vue";
import Projects from "./components/Projects.vue";
import Contact from "./components/Contact.vue";
import Footer from "./components/Footer.vue";
</script>
