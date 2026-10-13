<script setup>
import { projects } from '../data/portfolioData'
</script>

<template>
  <section id="projects" class="projects section-wrap section-pad">
    <div class="projects-top">
      <div class="section-heading"><p class="eyebrow">02 — SELECTED WORK</p><h2>Projects<br><em>with purpose.</em></h2></div>
      <p class="projects-note">Experiments and applications built to explore how technology can make everyday things simpler.</p>
    </div>
    <article v-for="project in projects" :key="project.number" class="project-row">
      <span class="project-number">{{ project.number }}</span>
      <div class="project-details">
        <p class="eyebrow">{{ project.type }}</p><h3>{{ project.title }}</h3>
        <p>{{ project.description }}</p><div class="tags">{{ project.stack }}</div>
      </div>
      <a class="project-link" :href="project.link" target="_blank" rel="noreferrer" :aria-label="`View ${project.title} on GitHub`">↗</a>
    </article>
  </section>
</template>
