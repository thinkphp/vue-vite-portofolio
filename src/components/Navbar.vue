<script setup>
import { ref } from 'vue'
import { navItems } from '../data/portfolioData'

defineProps({ isLight: { type: Boolean, default: false } })
defineEmits(['toggle-theme'])
const menuOpen = ref(false)
</script>

<template>
  <header class="topbar">
    <a class="wordmark" href="#home" aria-label="Home page">WA<span>.</span></a>
    <button class="menu-toggle" type="button" :aria-expanded="menuOpen" aria-label="Open menu" @click="menuOpen = !menuOpen">
      <span></span><span></span>
    </button>
    <nav :class="{ open: menuOpen }" aria-label="Main navigation">
      <a v-for="item in navItems" :key="item.id" :href="`#${item.id}`" @click="menuOpen = false">{{ item.label }}</a>
      <a class="nav-cta" href="#contact" @click="menuOpen = false">Let’s talk <span>↗</span></a>
      <button class="theme-toggle" type="button" :aria-label="`Switch to ${isLight ? 'dark' : 'light'} theme`" @click="$emit('toggle-theme')">
        <span>{{ isLight ? '☾' : '☼' }}</span>{{ isLight ? 'DARK' : 'LIGHT' }}
      </button>
    </nav>
  </header>
</template>
