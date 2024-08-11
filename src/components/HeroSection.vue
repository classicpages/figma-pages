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
        <li class="navbar-item"><span class="home">Home</span></li>
        <li class="navbar-item">Features</li>
        <li class="navbar-item">Pricing</li>
        <li class="navbar-item">Blog</li>
        <li class="navbar-item">Bē</li>
      </ul>
    </nav>
    
    <!-- Hero Content -->
    <div class="hero-content">
      <h1 class="startup">Startup 3</h1>
      <h2 class="forget">Forget About Code</h2>
      <p class="frame">Startup Framework gives you complete freedom over your creative <br> process - you don't have to think about any technical aspects. There <br> are no limits and absolutely no coding.</p>
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
  display: flex;
  flex-direction: column;
  justify-content: center;
  min-height: 100vh;
  position: relative;
  max-width: 100%;
}

/* Prevent horizontal scrolling */
body, html {
  margin: 0;
  padding: 0;
  overflow-x: hidden;
}

/* Ensure the width of the content fits the screen */
.container {
  max-width: 100%;
  overflow-x: hidden;
  box-sizing: border-box;
}

/* Apply this globally if needed */
* {
  box-sizing: border-box;
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


.startup {
  font-size: 17px;
  margin-bottom: 0.5rem;
  font-weight: 700;
}

.home {
  color: rgb(179, 170, 170);
}

.forget {
  font-size: 55px;
  margin-bottom: 1rem;
  font-weight: 600;
}

.frame {
  font-size: 18px;
  margin-bottom: 2rem;
  font-weight: 500;
  
}


.cta-button {
  background-color: #482BE7;
  color: white;
  border: none;
  padding: 0.75rem 2rem;
  font-size: 14px;
  cursor: pointer;
  border-radius: 19px;
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
