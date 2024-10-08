<template>
  <section class="hero">
    <div class="hero-content">
      <h2>YOUR DAILY CODING PARTNER</h2>
      <div class="project-preview">
        <img src="https://via.placeholder.com/50" alt="Project preview">
        <p>Latest Project: AI-powered Task Manager</p>
      </div>
    </div>
    <div class="hero-image">
      <img src="https://via.placeholder.com/400x300" alt="Programmer at work">
    </div>
    <div class="featured-project">
      <h3>Featured: Web App</h3>
      <img src="https://via.placeholder.com/100" alt="Web App">
    </div>
  </section>
</template>

<style scoped>
.hero {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 2rem;
  background-color: #e6f2f2;
  padding: 2rem;
  border-radius: 10px;
}

.hero-content {
  display: flex;
  flex-direction: column;
  justify-content: center;
}

h2 {
  font-size: 2.5rem;
  margin-bottom: 1rem;
}

.project-preview {
  display: flex;
  align-items: center;
  gap: 1rem;
  background-color: white;
  padding: 0.5rem;
  border-radius: 5px;
}

.hero-image img {
  width: 100%;
  height: auto;
  border-radius: 10px;
}

.featured-project {
  position: absolute;
  right: 2rem;
  bottom: 2rem;
  background-color: white;
  padding: 1rem;
  border-radius: 5px;
}
</style>