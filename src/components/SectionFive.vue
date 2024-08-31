<template>
  <section class="section-five">
    <h1>Our Happy Clients</h1>

    <div class="client-container">
      <div class="client good-morning flex-container">
        <div class="imgs">
          <img src="/src/assets/Mask (3).png" />
        </div>
        <div class="text-container">
          <div class="text">
            Get a fully retina-ready site when you build with Startup Framework.
            Websites look sharper and more gorgeous on devices with retina
            display support.
          </div>
          <p class="txt">Rayhan Curran</p>
        </div>
      </div>

      <div class="client good-morning flex-container">
        <div class="imgs">
          <img src="/src/assets/Mask (1).png" />
        </div>
        <div class="text-container">
          <div class="text">
            As a business targeting high net worth individuals, we were looking
            for a slick, cool, and minimalistic design for our website.
          </div>
          <p class="txt">Kayley Frame</p>
        </div>
      </div>

      <div class="client good-morning inline-block-container">
        <div class="imgs">
          <img src="/src/assets/Mask (2).png" />
        </div>
        <div class="text-container">
          <div class="text">
            The most important part of the Startup Framework is the samples.
          </div>
          <p class="txt">Gene Whitfield</p>
        </div>
      </div>

      <div class="client good-morning inline-block-container">
        <div class="imgs">
          <img src="/src/assets/Mask (3).png" />
        </div>
        <div class="text-container">
          <div class="text">
            I’ve built my website with Startup just in one day, and it was
            ready-to-go.
          </div>
          <p class="txt">Allan Kim</p>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "SectionFive",
};
</script>

<style scoped>
@import url("https://fonts.googleapis.com/css2?family=DM+Sans:ital,opsz,wght@0,9..40,100..1000;1,9..40,100..1000&display=swap");

.section-five {
  background-color: #1e0e62;
  color: white;
  display: flex;
  flex-direction: column;
  position: relative;
  max-width: 100%;
  padding: 50px 20px;
  max-height: 100vh;
}

h1 {
  font-weight: 700;
  text-align: left;
  margin-left: 215px;
  margin-bottom: 50px;
  width: 364px;
  height: 52px;
  font-family: 'DM Sans', sans-serif;
  font-size: 42px;
  line-height: 52px;
  letter-spacing: -0.4px;
}

.client-container {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  gap: 20px;
}

.client {
  width: 470px;
  height: 237px;
  background-color: #1e0e62;
  color: white;
  box-sizing: border-box;
  border: 2px solid gray;
  border-radius: 10px;
  display: flex;
  align-items: center;
  justify-content: space-between;
}

.flex-container {
  display: flex;
  align-items: center;
}

.inline-block-container {
  vertical-align: middle;
}

.imgs img {
  width: 70px;
  height: 70px;
  border-radius: 10px 0px 0px 0px;
  padding: 36px 30px 131px;
}

.text-container {
  width: 307px;
  margin-left: 30px;
  font-family: "DM Sans", sans-serif;
  font-size: 18px;
  font-weight: 500;
  line-height: 28px;
}

.text {
  line-height: 1.5;
  text-align: left;
  width: 307px;
  height: 140px;
  font-family: "DM Sans", sans-serif;
  font-size: 18px;
  font-weight: 500;
  line-height: 28px;
}

.txt {
  margin-top: 13px;
  font-family: "DM Sans", sans-serif;
  color: #ffffff;
  font-size: 14px;
  font-weight: 700;
  line-height: 26px;
  letter-spacing: 2px;
}

/* Responsive styling */
@media (max-width: 1440px) {
  h1 {
    margin-left: 180px;
  }
  .client-container {
    gap: 15px;
  }
}

@media (max-width: 1200px) {
  h1 {
    margin-left: 150px;
  }
}

@media (max-width: 1024px) {
  h1 {
    margin-left: 100px;
  }
}

@media (max-width: 1000px) {
  h1 {
    margin-left: 80px;
    font-size: 36px;
  }
  .client {
    width: 100%;
    max-width: 90%;
  }
}

@media (max-width: 900px) {
  h1 {
    margin-left: 60px;
    font-size: 32px;
  }
  .client {
    width: 100%;
    max-width: 90%;
  }
}

@media (max-width: 810px) {
  h1 {
    margin-left: 30px;
    font-size: 28px;
    text-align: center;
  }
  .client {
    width: 100%;
    max-width: 90%;
  }
}

@media (max-width: 768px) {
  h1 {
    margin-left: 0;
    font-size: 24px;
    text-align: center;
  }
  .client {
    width: 100%;
    max-width: 90%;
  }
  .imgs img {
    width: 60px;
    height: 60px;
  }
}

@media (max-width: 480px) {
  h1 {
    font-size: 22px;
    text-align: center;
  }
  .client-container {
    flex-direction: column;
    align-items: center;
  }
  .client {
    width: 100%;
    max-width: 90%;
  }
  .imgs img {
    width: 50px;
    height: 50px;
  }
  .text-container {
    width: 100%;
  }
}
</style>
