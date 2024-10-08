<script setup lang="ts">
import { ref } from 'vue'

const skills = ref([
  'HTML5', 'CSS3', 'JavaScript', 'TypeScript',
  'Vue.js', 'React', 'Node.js', 'Express',
  'MongoDB', 'SQL', 'Git', 'Webpack',
  'Responsive Design', 'RESTful APIs'
])
</script>

<template>
  <section id="skills">
    <h2>Skills</h2>
    <ul class="skills-list">
      <li v-for="skill in skills" :key="skill" class="skill-item">
        {{ skill }}
      </li>
    </ul>
  </section>
</template>

<style scoped>
.skills-list {
  display: flex;
  flex-wrap: wrap;
  gap: 1rem;
  justify-content: center;
  list-style-type: none;
  padding: 0;
}

.skill-item {
  background-color: #f0f0f0;
  padding: 0.5rem 1rem;
  border-radius: 4px;
  font-weight: bold;
}
</style>