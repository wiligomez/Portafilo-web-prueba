<script setup lang="ts">
const projects = [
  { name: 'Web App', image: 'https://via.placeholder.com/150' },
  { name: 'Mobile App', image: 'https://via.placeholder.com/150' },
  { name: 'API', image: 'https://via.placeholder.com/150' },
  { name: 'Data Analysis', image: 'https://via.placeholder.com/150' },
]
</script>

<template>
  <section class="projects-grid">
    <div v-for="project in projects" :key="project.name" class="project-card">
      <img :src="project.image" :alt="project.name">
      <h3>{{ project.name }}</h3>
    </div>
  </section>
</template>

<style scoped>
.projects-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
  gap: 1rem;
}

.project-card {
  background-color: white;
  padding: 1rem;
  border-radius: 5px;
  box-shadow: 0 2px 4px rgba(0,0,0,0.1);
}

.project-card img {
  width: 100%;
  height: auto;
  border-radius: 5px;
}

.project-card h3 {
  margin-top: 0.5rem;
  font-size: 1rem;
}
</style>