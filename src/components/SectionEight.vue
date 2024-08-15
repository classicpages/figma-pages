<template>
  <section class="section-eight">
    <div class="text-container">
      <h1 class="start">Startup Crew</h1>
      <p class="para">
        The most important part of the Startup Framework is the samples. <br />
        The samples form a set of 25 usable pages you can use as is or you can
        add 
        new blocks from UI Kit.
      </p>
    </div>
    <div class="image-container">
      <div class="image-card">
        <div class="image-placeholder">
          <img src="/src/assets/Mask (1).png" />
        </div>
        <h2>Leah Salomon</h2>
        <p>UI Designer</p>
      </div>

      <div class="image-card">
        <div class="image-placeholder">
          <img src="/src/assets/Mask (2).png" />
        </div>
        <h2>Colin Timmons</h2>
        <p>UI Designer</p>
      </div>

      <div class="image-card">
        <div class="image-placeholder">
          <img src="/src/assets/Mask (3).png" />
        </div>
        <h2>Miguel Osborne</h2>
        <p>UI Designer</p>
      </div>

      <div class="image-card">
        <div class="image-placeholder">
          <img src="/src/assets/Mask (1).png" />
        </div>
        <h2>Taylor Simon</h2>
        <p>UI Designer</p>
      </div>

      <div class="image-card">
        <div class="image-placeholder">
          <img src="/src/assets/Mask (2).png" />
        </div>
        <h2>Steven MacAlister</h2>
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
.section-eight {
  background-color: rgb(15, 15, 80);
  color: white;
  padding-left: 90px;
  padding-top: 10px;
  max-height: 100%;
  position: relative;
  max-width: 100%;
}

.text-container {
  text-align: left;
  margin-bottom: 20px;
}

.image-container {
  display: flex;
  flex-wrap: wrap;
  height: 543px;
}

.image-card {
  flex-direction: column;
  align-items: left;
  width: 320px;
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
  margin-top: 20px;
  margin-bottom: 20px;
  font-size: 22px;
  font-weight: 300;
  width: 754px;
height: 96px;
line-height: 32px;
text-align: left;

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
