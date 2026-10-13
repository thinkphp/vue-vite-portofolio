<script setup>
import portrait from '../assets/cover.jpeg'
</script>

<template>
  <section id="home" class="hero section-wrap">
    <div class="hero-copy">
      <p class="eyebrow"><span class="status-dot"></span> PORTFOLIO · 2026</p>
      <h1>From idea to<br><em>working software</em><span class="accent">.</span></h1>
      <p class="hero-intro">Hi, I’m <strong>Warren Buffett Adrian</strong> — a software developer passionate about useful products, thoughtful code, and turning ideas into digital experiences.</p>
      <div class="hero-actions">
        <a class="button button-dark" href="#projects">Explore my work <span>↘</span></a>
        <a class="text-link" href="mailto:buffett@gmail.com">Send me a message <span>↗</span></a>
      </div>
      <div class="hero-meta"><span>JAVA · FULL STACK</span><span>BASED IN ROMANIA</span></div>
    </div>
    <div class="hero-visual">
      <div class="image-frame"><img :src="portrait" alt="Portrait of Warren Buffett Adrian"><span class="image-index">01 / 04</span></div>
      <div class="orbit orbit-one"></div><div class="orbit orbit-two"></div>
      <div class="floating-note"><span>✳</span><div>Curiosity<br><b>in progress</b></div></div>
      <span class="vertical-label">DESIGN · BUILD · LEARN</span>
    </div>
    <a class="scroll-cue" href="#about"><span></span> SCROLL TO EXPLORE</a>
  </section>
</template>
