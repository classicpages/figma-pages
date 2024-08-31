<template>
  <section class="section-eight">
    <div class="text-container">
      <h1 class="start">Startup Crew</h1>
      <p class="para">
        The most important part of the Startup Framework is the samples. The
        samples form a set of 25 usable pages you can use as is or you can add
        new blocks from UI Kit.
      </p>
    </div>
    <div class="image-container">
      <div class="image-card">
        <div class="image-placeholder">
          <img src="/src/assets/Mask (1).png" />
        </div>
        <h2 class="names">Leah Salomon</h2>
        <p>UI Designer</p>
      </div>

      <div class="image-card">
        <div class="image-placeholder">
          <img src="/src/assets/Mask (2).png" />
        </div>
        <h2 class="names">Colin Timmons</h2>
        <p>UI Designer</p>
      </div>

      <div class="image-card">
        <div class="image-placeholder">
          <img src="/src/assets/Mask (3).png" />
        </div>
        <h2 class="names">Miguel Osborne</h2>
        <p>UI Designer</p>
      </div>

      <div class="image-card">
        <div class="image-placeholder">
          <img src="/src/assets/Mask (1).png" />
        </div>
        <h2 class="names">Taylor Simon</h2>
        <p>UI Designer</p>
      </div>

      <div class="image-card">
        <div class="image-placeholder">
          <img src="/src/assets/Mask (2).png" />
        </div>
        <h2 class="names">Steven MacAlister</h2>
        <p>UI Designer</p>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "SectionEight",
};
</script>

<style scoped>
@import url("https://fonts.googleapis.com/css2?family=DM+Sans:ital,opsz,wght@0,9..40,100..1000;1,9..40,100..1000&display=swap");

.section-eight {
  background-color: rgb(15, 15, 80);
  color: white;
  max-height: 100%;
  position: relative;
  max-width: 100%;
  padding: 20px;
}

.text-container {
  text-align: left;
  margin-bottom: 50px;
  padding: 20px;
  max-width: 100%;
}

.image-container {
  display: flex;
  flex-wrap: wrap;
  justify-content: space-between;
  padding: 20px;
}

.image-card {
  flex-direction: column;
  align-items: left;
  width: 154px;
  height: 241.2px;
  margin-bottom: 20px;
}

.start {
  font-size: 35px;
  font-weight: 700;
  line-height: 52px;
  letter-spacing: -0.4px;
}

.para {
  font-weight: 300;
  font-size: 22px;
  line-height: 32px;
  font-family: "DM Sans";
}

.names {
  margin-top: 17px;
  width: 145px;
  height: 32px;
  font-family: "DM Sans", sans-serif;
  font-size: 22px;
  text-align: left;
  padding-bottom: 8.19px;
}

/* Media Queries for Responsiveness */

/* For 1440px screens and larger */
@media (max-width: 1440px) {
  .text-container {
    max-width: 85%;
  }

  .image-card {
    width: calc(20% - 20px);
  }
}

/* For 1200px screens */
@media (max-width: 1200px) {
  .text-container {
    max-width: 80%;
  }

  .image-card {
    width: calc(25% - 20px);
  }
}

/* For 1024px screens */
@media (max-width: 1024px) {
  .text-container {
    max-width: 75%;
  }

  .image-card {
    width: calc(33.33% - 20px);
  }
}

/* For 1000px screens */
@media (max-width: 1000px) {
  .text-container {
    max-width: 70%;
  }

  .image-card {
    width: calc(33.33% - 15px);
  }
}

/* For 900px screens */
@media (max-width: 900px) {
  .text-container {
    max-width: 65%;
  }

  .image-card {
    width: calc(50% - 15px);
  }
}

/* For 810px screens */
@media (max-width: 810px) {
  .text-container {
    max-width: 60%;
  }

  .image-card {
    width: calc(50% - 10px);
  }
}

/* For 768px screens */
@media (max-width: 768px) {
  .text-container {
    max-width: 100%;
    padding: 15px;
  }

  .image-card {
    width: calc(50% - 10px);
  }
}

/* For 480px screens */
@media (max-width: 480px) {
  .text-container {
    max-width: 100%;
    padding: 10px;
  }

  .image-card {
    width: calc(100% - 10px);
  }

  .start {
    font-size: 28px;
  }

  .para {
    font-size: 18px;
  }
}
</style>
