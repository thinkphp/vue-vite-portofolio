<script setup>
import { journey } from '../data/portfolioData'
</script>

<template>
  <section class="path section-pad">
    <div class="section-wrap path-inner">
      <div class="section-heading"><p class="eyebrow">03 — THE JOURNEY</p><h2>Always<br><em>evolving.</em></h2></div>
      <div class="timeline">
        <div v-for="(item, index) in journey" :key="item.label" class="timeline-item">
          <span>{{ item.label }}</span><div><h3>{{ item.title }}</h3><p>{{ item.description }}</p></div><b>{{ String(index + 1).padStart(2, '0') }}</b>
        </div>
      </div>
    </div>
  </section>
</template>
