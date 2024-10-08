<template>
  <section class="feature-project">
    <img src="https://via.placeholder.com/300x200" alt="Feature project">
    <div class="project-info">
      <h2>Full Stack Web Application</h2>
      <p>A complete web solution with front-end, back-end, and database integration.</p>
      <div class="price">Starting at $5000</div>
      <button>Learn more</button>
    </div>
  </section>
</template>

<style scoped>
.feature-project {
  display: flex;
  gap: 2rem;
  background-color: #f0f0f0;
  padding: 2rem;
  border-radius: 10px;
}

.feature-project img {
  width: 300px;
  height: 200px;
  object-fit: cover;
  border-radius: 5px;
}

.project-info {
  display: flex;
  flex-direction: column;
  gap: 1rem;
}

h2 {
  font-size: 1.5rem;
}

.price {
  font-weight: bold;
}

button {
  align-self: flex-start;
  padding: 0.5rem 1rem;
  background-color: #333;
  color: white;
  border: none;
  border-radius: 5px;
  cursor: pointer;
}
</style>