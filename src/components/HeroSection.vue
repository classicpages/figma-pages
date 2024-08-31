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
      <p class="frame">Startup Framework gives you complete freedom over your creative 
        <br> process - you don't have to think about any technical aspects.
         There are no limits and absolutely no coding.</p>
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
  background-color: #2F1893;
} 

* {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}

.navbar {
  position: absolute;
  top: 0;
  width: 100%;
  padding: 1rem;
  color: white;
  display: flex;
  justify-content: center; /* Center align navbar items */
  align-items: center;
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
  justify-content: center; /* Center align navbar items */
  margin: 0;
  padding: 0;
}

.navbar-item {
  margin: 0 1rem; /* Adjusted margin for better spacing */
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

/* For screen sizes up to 480px */
@media (max-width: 480px) {
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
  
  .forget {
    font-size: 32px;
  }
  
  .frame {
    font-size: 16px;
  }

  .cta-button {
    padding: 0.5rem 1.5rem;
    font-size: 12px;
  }
}

/* For screen sizes between 481px and 768px */
@media (min-width: 481px) and (max-width: 768px) {
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
  
  .forget {
    font-size: 40px;
  }
  
  .frame {
    font-size: 17px;
  }

  .cta-button {
    padding: 0.6rem 1.8rem;
    font-size: 13px;
  }
}

/* For screen sizes between 769px and 810px */
@media (min-width: 769px) and (max-width: 810px) {
  .forget {
    font-size: 44px;
  }
  
  .frame {
    font-size: 17px;
  }

  .cta-button {
    padding: 0.65rem 1.9rem;
    font-size: 13px;
  }
}

/* For screen sizes between 811px and 900px */
@media (min-width: 811px) and (max-width: 900px) {
  .forget {
    font-size: 48px;
  }
  
  .frame {
    font-size: 18px;
  }

  .cta-button {
    padding: 0.7rem 2rem;
    font-size: 14px;
  }
}

/* For screen sizes between 901px and 1000px */
@media (min-width: 901px) and (max-width: 1000px) {
  .forget {
    font-size: 50px;
  }
  
  .frame {
    font-size: 18px;
  }

  .cta-button {
    padding: 0.75rem 2.1rem;
    font-size: 14px;
  }
}

/* For screen sizes between 1001px and 1024px */
@media (min-width: 1001px) and (max-width: 1024px) {
  .forget {
    font-size: 52px;
  }
  
  .frame {
    font-size: 18px;
  }

  .cta-button {
    padding: 0.8rem 2.2rem;
    font-size: 14px;
  }
}

/* For screen sizes between 1025px and 1200px */
@media (min-width: 1025px) and (max-width: 1200px) {
  .forget {
    font-size: 55px;
  }
  
  .frame {
    font-size: 18px;
  }

  .cta-button {
    padding: 0.8rem 2.3rem;
    font-size: 14px;
  }
}

/* For screen sizes between 1201px and 1440px */
@media (min-width: 1201px) and (max-width: 1440px) {
  .forget {
    font-size: 55px;
  }
  
  .frame {
    font-size: 19px;
  }

  .cta-button {
    padding: 0.85rem 2.5rem;
    font-size: 15px;
  }
}

/* For screen sizes larger than 1440px */
@media (min-width: 1441px) {
  .forget {
    font-size: 58px;
  }
  
  .frame {
    font-size: 19px;
  }

  .cta-button {
    padding: 0.85rem 2.8rem;
    font-size: 15px;
  }
}
</style>
