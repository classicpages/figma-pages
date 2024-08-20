<template>
  <section class="section-five">
    <h1>OUR HAPPY CLIENTS</h1>

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
            <p class="txt">Rayhan Curran</p>
          </div>
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
            <p class="txtK">Kayley Frame</p>
          </div>
        </div>
      </div>

      <div class="client good-morning inline-block-container">
        <div class="imgs">
          <img src="/src/assets/Mask (2).png" />
        </div>
        <div class="text-container">
          <div class="text">
            The most important part of the Startup Framework is the samples.
            <p class="txtG">Gene Whitfield</p>
          </div>
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
            <p class="txtA">Allan Kim</p>
          </div>
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
.section-five {
  background-color: #1e0e62;
  color: white;
  display: flex;
  flex-direction: column;
  position: relative;
  max-width: 100%;
  padding: 50px 20px;
}

h1 {
  font-size: 26px;
  font-weight: 700;
  text-align: left;
  margin-left: 215px;
  margin-bottom: 50px;
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
}

.flex-container {
  display: flex;
}

.inline-block-container {
  display: inline-block;
}

.imgs img {
  width: 70px;
  height: 70px;
  margin: 36px 0 0 35px;
  border-radius: 10px 0px 0px 0px;
}

.text-container {
  width: 307px;
  height: 140px;
  margin: 35px 0 0 30px;
}

.text {
  font-size: 14px;
  line-height: 1.5;
}

.txt,
.txtK,
.txtG,
.txtA {
  font-weight: 700;
  margin-top: 15px;
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

@media (max-width: 768px) {
  h1 {
    text-align: center;
    margin-left: 0;
  }
  .client {
    width: 100%;
    margin: 0 auto;
  }
  .imgs img {
    margin-left: 20px;
  }
}

@media (max-width: 480px) {
  h1 {
    font-size: 22px;
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
    margin-left: 10px;
  }
}
</style>
