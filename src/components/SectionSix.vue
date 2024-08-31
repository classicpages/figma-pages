<template>
  <section class="section-six">
    <div class="content">
      <div class="easy">
        <h1>Easy to setup. Easy to maintain</h1>
      </div>
      <p>
        Bootstrap is a widely-used, sleek, intuitive, and powerful front-end
        framework for faster and easier web development.
      </p>
      <div class="button-wrapper">
        <img
          src="/src/assets/Icon - Fill (1).png"
          class="button-icon"
          alt="Icon"
        />
        <button class="get-started-button">Get Started</button>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "SectionSix",
};
</script>

<style scoped>
@import url("https://fonts.googleapis.com/css2?family=DM+Sans:ital,opsz,wght@0,9..40,100..1000;1,9..40,100..1000&display=swap");

.section-six {
  background-image: url("/src/assets/Rectangle.png");
  background-size: cover;
  background-position: center;
  color: white;
  display: flex;
  justify-content: center;
  align-items: center;
  position: relative;
  width: 100%;
  height: 100vh;
  text-align: center;
  background-color: #2f1893;
}

.content {
  text-align: center;
  height: 277px;
  margin-bottom: 100px;
}

p {
  margin-bottom: 40px;
  width: 518px;
  height: 96px;
  font-family: 'DM Sans', sans-serif;
  font-size: 22px;
  line-height: 32px;
  text-align: center;
  margin-left: auto;
  margin-right: auto;
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
  margin-bottom: 100px;
}

.easy {
  width: 770px;
  height: 161px;
  font-family: "DM Sans";
  font-size: 58px;
  line-height: 70px;
  letter-spacing: -1px;
  text-align: center;
  margin: 0 auto;
}

.get-started-button {
  background-color: #25dac5;
  color: white;
  border: none;
  border-radius: 22px;
  padding: 15px 30px;
  font-size: 16px;
  cursor: pointer;
  margin-bottom: 100px;
}

.get-started-button:hover {
  background-color: #84d6cd;
}

/* Responsive styles */
@media (max-width: 1440px) {
  .easy {
    font-size: 52px;
    line-height: 64px;
  }

  p {
    width: 480px;
    font-size: 20px;
    line-height: 30px;
  }
}

@media (max-width: 1200px) {
  .easy {
    font-size: 48px;
    line-height: 60px;
  }

  p {
    width: 400px;
    font-size: 18px;
    line-height: 28px;
  }

  .get-started-button {
    padding: 14px 28px;
  }
}

@media (max-width: 1024px) {
  .easy {
    font-size: 42px;
    line-height: 54px;
  }

  p {
    width: 350px;
    font-size: 18px;
    line-height: 28px;
  }

  .get-started-button {
    padding: 14px 26px;
  }
}

@media (max-width: 1000px) {
  .easy {
    font-size: 40px;
    line-height: 52px;
  }

  p {
    width: 330px;
    font-size: 17px;
    line-height: 26px;
  }

  .get-started-button {
    padding: 13px 25px;
  }
}

@media (max-width: 900px) {
  .easy {
    font-size: 36px;
    line-height: 48px;
  }

  p {
    width: 300px;
    font-size: 16px;
    line-height: 24px;
  }

  .get-started-button {
    padding: 12px 24px;
  }
}

@media (max-width: 810px) {
  .easy {
    font-size: 34px;
    line-height: 46px;
  }

  p {
    width: 280px;
    font-size: 16px;
    line-height: 24px;
  }

  .get-started-button {
    padding: 12px 23px;
  }
}

@media (max-width: 768px) {
  .easy {
    font-size: 32px;
    line-height: 42px;
  }

  p {
    width: 270px;
    font-size: 15px;
    line-height: 22px;
  }

  .get-started-button {
    padding: 12px 22px;
    font-size: 15px;
  }
}

@media (max-width: 480px) {
  .easy {
    font-size: 28px;
    line-height: 38px;
    width: 90%;
  }

  p {
    width: 80%;
    font-size: 14px;
    line-height: 22px;
  }

  .get-started-button {
    padding: 10px 20px;
    font-size: 14px;
  }

  .button-icon {
    width: 40px;
    height: 40px;
  }
}
</style>
