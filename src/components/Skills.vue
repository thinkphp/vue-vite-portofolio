<script setup>
import { skills } from '../data/portfolioData'
</script>

<template>
  <section class="skills-band">
    <div class="skills-label">MY TOOLKIT <span>✳</span></div>
    <div class="skill-list"><span v-for="skill in skills" :key="skill">{{ skill }}</span></div>
  </section>
</template>
