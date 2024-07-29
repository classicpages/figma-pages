<template>
  <div class="hero-section">
    <!-- Navbar -->
    <nav class="navbar">
      <div class="navbar-toggle" @click="toggleNavbar">
        <span class="bar"></span>
        <span class="bar"></span>
        <span class="bar"></span>
      </div>
      <ul :class="['navbar-menu', { 'active': isNavbarOpen }]">
        <li class="navbar-item">Home</li>
        <li class="navbar-item">Features</li>
        <li class="navbar-item">Pricing</li>
        <li class="navbar-item">Blog</li>
        <li class="navbar-item">Bē</li>
      </ul>
    </nav>
    
    <!-- Hero Content -->
    <div class="hero-content">
      <h1>Startup 3</h1>
      <h2>Forget About Code.</h2>
      <p>Startup Framework gives you complete freedom over your creative process - you don't have to think about any technical aspects. There are no limits and absolutely no coding.</p>
      <button class="cta-button">Create an Account</button>
    </div>
  </div>
</template>

<script>
export default {
  name: 'HeroSection',
  data() {
    return {
      isNavbarOpen: false
    }
  },
  methods: {
    toggleNavbar() {
      this.isNavbarOpen = !this.isNavbarOpen;
    }
  }
}
</script>

<style scoped>
.hero-section {
  background-image: url('@/assets/4c269f57807850115899b4611a2bf3ba.jpeg');
  background-size: cover;
  background-position: center;
  background-repeat: no-repeat;
  color: white;
  text-align: center;
  padding: 2rem;
  display: flex;
  flex-direction: column;
  justify-content: center;
  min-height: 100vh;
  position: relative;
}

.navbar {
  position: absolute;
  top: 0;
  width: 100%;
  padding: 1rem;
  color: white;
  display: flex;
  flex-direction: column;
}

.navbar-toggle {
  display: none;
  flex-direction: column;
  cursor: pointer;
}

.navbar-toggle .bar {
  background-color: white;
  height: 3px;
  width: 25px;
  margin: 5px 0;
}

.navbar-menu {
  list-style: none;
  display: flex;
  justify-content: center;
  margin: 0;
  padding: 0;
}

.navbar-item {
  margin: 0 1rem;
}

.hero-content {
  margin-top: 6rem;
}

.hero-content h1 {
  font-size: 3rem;
  margin-bottom: 0.5rem;
}

.hero-content h2 {
  font-size: 2rem;
  margin-bottom: 1rem;
}

.hero-content p {
  font-size: 1.2rem;
  margin-bottom: 2rem;
}

.cta-button {
  background-color: blue;
  color: white;
  border: none;
  padding: 0.75rem 2rem;
  font-size: 18px;
  cursor: pointer;

  border-radius: 15px;
}

.cta-button:hover {
  opacity: 0.8;
}

/* Responsive Styles */
@media (max-width: 768px) {
  .navbar-menu {
    display: none;
    flex-direction: column;
    width: 100%;
    text-align: center;
  }

  .navbar-menu.active {
    display: flex;
  }

  .navbar-toggle {
    display: flex;
  }
}
</style>
