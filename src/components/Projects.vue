<script setup lang="ts">
import { ref } from 'vue'

interface Project {
  title: string
  description: string
  technologies: string[]
  link: string
}

const projects = ref<Project[]>([
  {
    title: 'Project 1',
    description: 'A brief description of your first project.',
    technologies: ['Vue.js', 'TypeScript', 'Vuex'],
    link: 'https://github.com/yourusername/project1'
  },
  {
    title: 'Project 2',
    description: 'A brief description of your second project.',
    technologies: ['React', 'Node.js', 'MongoDB'],
    link: 'https://github.com/yourusername/project2'
  },
  // Add more projects as needed
])
</script>

<template>
  <section id="projects">
    <h2>Projects</h2>
    <div class="project-grid">
      <div v-for="project in projects" :key="project.title" class="project-card">
        <h3>{{ project.title }}</h3>
        <p>{{ project.description }}</p>
        <div class="technologies">
          <span v-for="tech in project.technologies" :key="tech" class="tech-tag">{{ tech }}</span>
        </div>
        <a :href="project.link" target="_blank" rel="noopener noreferrer">View Project</a>
      </div>
    </div>
  </section>
</template>

<style scoped>
.project-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
  gap: 2rem;
}

.project-card {
  border: 1px solid #ddd;
  border-radius: 8px;
  padding: 1rem;
  display: flex;
  flex-direction: column;
  gap: 0.5rem;
}

.technologies {
  display: flex;
  flex-wrap: wrap;
  gap: 0.5rem;
}

.tech-tag {
  background-color: #42b883;
  color: white;
  padding: 0.2rem 0.5rem;
  border-radius: 4px;
  font-size: 0.8rem;
}
</style>