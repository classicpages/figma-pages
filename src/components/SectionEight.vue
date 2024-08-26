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
}

.text-container {
  text-align: left;
  margin-bottom: 50px;
  width: 754px;
  height: 179px;
  top: 100px;
  left: 115px;
  gap: 0px;
  opacity: 0px;
  margin-left: 115px;
  padding-top: 100px;
}

.image-container {
  display: flex;
  flex-wrap: wrap;
  height: 543px;
  width: 764px;
  top: 349px;
  left: 115px;
  margin-left: 115px;
  padding-top: 50px;
  padding-bottom: 50px;
}

.image-card {
  flex-direction: column;
  align-items: left;
  width: 154px;
  height: 241.2px;
  top: 349px;
  margin-right: 70px;
  opacity: 0px;
}

.start {
  margin-top: 40px;
  margin-bottom: 20px;
  font-size: 35px;
  font-weight: 700;
  width: 265px;
  height: 52px;
  font-size: 42px;
  line-height: 52px;
  letter-spacing: -0.4000000059604645px;
  text-align: left;
}

.para {
  margin-top: 31px;
  margin-bottom: 70px;
  font-weight: 300;
  width: 754px;
  height: 96px;
  line-height: 32px;
  width: 754px;
  height: 96px;
  top: 183px;
  left: 115px;
  font-family: "DM Sans";
  font-size: 22px;
  line-height: 32px;
  text-align: left;
}

.names {
  margin-top: 17px;
  width: 145px;
  height: 32px;
  font-family: "DM Sans" sans-serif;
  font-size: 22px;
  text-align: left;
  padding-bottom: 8.19px;
}

@media (max-width: 768px) {
  .image-card {
    flex: 1 1 calc(50% - 20px);
  }
}

@media (max-width: 480px) {
  .image-card {
    flex: 1 1 100%;
  }
}
</style>
