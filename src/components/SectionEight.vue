<template>
    <section class="section-eight">
      <div class="text-container">
        <h1>Startup Crew</h1>
        <p>
          The most important part of the Startup Framework is the samples. <br> The samples form a set of 25 usable pages you can use as is or you can add <br> new blocks from UI Kit.
        </p>
      </div>
      <div class="image-container">
        <div class="image-card">
          <div class="image-placeholder"><img src="/src/assets/Mask (1).png"></div>
          <h2>Leah Salomon</h2>
          <p>UI Designer</p>
        </div>

        <div class="image-card">
          <div class="image-placeholder"><img src="/src/assets/Mask (2).png"></div>
          <h2>Colin Timmons</h2>
          <p>UI Designer</p>
        </div>

        <div class="image-card">
          <div class="image-placeholder"><img src="/src/assets/Mask (3).png"></div>
          <h2>Miguel Osborne</h2>
          <p>UI Designer</p>
        </div>

        <div class="image-card">
          <div class="image-placeholder"><img src="/src/assets/Mask (1).png"></div>
          <h2>Taylor Simon</h2>
          <p>UI Designer</p>
        </div>

        <div class="image-card">
          <div class="image-placeholder"><img src="/src/assets/Mask (2).png"></div>
          <h2>Steven MacAlister</h2>
          <p>UI Designer</p>
        </div>

      </div>
    </section>
  </template>
  
  <script>
  export default {
    name: 'SectionEight',
  };
  </script>
  
  <style scoped>
  .section-eight {
    background-color: rgb(15, 15, 80);
    color: white;
    padding: 20px;
  }
  
  .text-container {
    text-align: left;
    margin-bottom: 20px;
  }
  
  .image-container {
    display: flex;
    flex-wrap: wrap;
    gap: 20px;
  }
  
  .image-card { 
    flex-direction: column;
    align-items: left;
  }
  
  .image-placeholder {
    width: 100px;
    height: 100px;
  }
  
  h1, h2, p {
    margin-top: 10px;
    margin-bottom: 10px;
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
  