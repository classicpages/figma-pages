<template>
  <section class="section-six">
    <div class="content">
    <div class="easy"><h1>Easy to setup. Easy to maintain</h1></div>
      <p>Bootstrap is a widely-used, sleek, intuitive, and<br> powerful front-end framework for faster and <br> easier web development.</p>
      <div class="button-wrapper">
        <img src="/src/assets/Icon - Fill (1).png" class="button-icon" alt="Icon" />
        <button class="get-started-button">Get Started</button>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: 'SectionSix'
}
</script>

<style scoped>
.section-six {
  background-image: url('/src/assets/Rectangle.png');
  background-size: cover;
  background-position: center;
  color: white;
  display: flex;
  justify-content: center;
  align-items: center;
  position: relative;
  width: 100%;
  height: 605px;
  text-align: center;
  background-color: #2F1893;
}

.content {
  text-align: center; 
  height: 277px;
}

h1 {
  margin-bottom: 20px;
  font-weight: 500;
  max-width: 770px;
  max-height: 161px;
  font-size: 58px;
  line-height: 70px;
  letter-spacing: -1px;
  text-align: center;
}

p {
  font-size: 15px;
  margin-bottom: 40px;
}

.button-wrapper {
  display: flex;
  justify-content: center;
  align-items: center;
  position: relative;
}

.button-icon {
  width: 50px;
  height: 50px;
  margin-right: 10px; 
}

.easy {
 width: 770px;
  height: 161px;

}

.get-started-button {
  background-color: #25DAC5;
  color: white;
  border: none;
  border-radius: 22px;
  padding: 15px 30px;
  font-size: 16px;
  cursor: pointer;
}

.get-started-button:hover {
  background-color: #84d6cd;
}

@media (max-width: 768px) {
  .section-six {
    padding: 20px;
  }

  h1 {
    font-size: 28px;
  }

  p {
    font-size: 18px;
  }

  .get-started-button {
    padding: 12px 24px;
    font-size: 16px;
  }
}

@media (max-width: 480px) {
  h1 {
    font-size: 24px;
  }

  p {
    font-size: 16px;
  }

  .get-started-button {
    padding: 10px 20px;
    font-size: 14px;
  }
}
</style>
