<script setup lang="ts">
import Header from './components/Header.vue'
import HeroSection from './components/HeroSection.vue'
import ProjectsGrid from './components/ProjectsGrid.vue'
import BrandMission from './components/BrandMission.vue'
import FeatureProject from './components/FeatureProject.vue'
</script>

<template>
  <div class="app">
    <Header />
    <main>
      <HeroSection />
      <ProjectsGrid />
      <BrandMission />
      <FeatureProject />
    </main>
  </div>
</template>

<style>
.app {
  max-width: 1200px;
  margin: 0 auto;
  padding: 1rem;
  font-family: Arial, sans-serif;
}

main {
  display: flex;
  flex-direction: column;
  gap: 2rem;
}
</style>