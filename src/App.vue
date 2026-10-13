<script setup>
import { onMounted, ref, watch } from 'vue'
import Navbar from './components/Navbar.vue'
import Hero from './components/Hero.vue'
import About from './components/About.vue'
import Skills from './components/Skills.vue'
import Projects from './components/Projects.vue'
import Journey from './components/Journey.vue'
import Contact from './components/Contact.vue'
import Footer from './components/Footer.vue'

const isLight = ref(false)

function applyTheme() {
  document.documentElement.dataset.theme = isLight.value ? 'light' : 'dark'
  localStorage.setItem('portfolio-theme', isLight.value ? 'light' : 'dark')
}

function toggleTheme() {
  isLight.value = !isLight.value
}

onMounted(() => {
  isLight.value = localStorage.getItem('portfolio-theme') === 'light'
  applyTheme()
})

watch(isLight, () => applyTheme())
</script>

<template>
  <div class="site-shell">
    <Navbar :is-light="isLight" @toggle-theme="toggleTheme" />
    <main>
      <Hero />
      <About />
      <Skills />
      <Projects />
      <Journey />
      <Contact />
    </main>
    <Footer />
  </div>
</template>
