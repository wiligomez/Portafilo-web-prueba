<template>
  <header>
    <h1>CODER</h1>
    <nav>
      <a href="#projects">Projects</a>
      <a href="#about">About</a>
      <a href="#skills">Skills</a>
      <a href="#contact">Contact</a>
    </nav>
    <div class="actions">
      <button>EN</button>
      <button>Contact us</button>
    </div>
  </header>
</template>

<style scoped>
header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 1rem 0;
}

h1 {
  font-size: 1.5rem;
  font-weight: bold;
}

nav {
  display: flex;
  gap: 1rem;
}

nav a {
  text-decoration: none;
  color: #333;
}

.actions {
  display: flex;
  gap: 0.5rem;
}

button {
  padding: 0.5rem 1rem;
  border: none;
  background-color: #f0f0f0;
  cursor: pointer;
}

button:last-child {
  background-color: #333;
  color: white;
}
</style>