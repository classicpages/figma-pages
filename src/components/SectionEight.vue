<template>
    <section class="section-eight">
      <div class="text-container">
        <h1>Startup Crew</h1>
        <p>
          The most important part of the Startup Framework is the samples. The samples form a set of 25 usable pages you can use as is or you can add new blocks from UI Kit.
        </p>
      </div>
      <div class="image-container">
        <div v-for="n in 5" :key="n" class="image-card">
          <!-- Placeholder for images -->
          <div class="image-placeholder"></div>
          <h2>Leah Salomon</h2>
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
    background-color: rgb(98, 98, 170);
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
    justify-content: flex-start;
  }
  
  .image-card { 
    flex-direction: column;
    align-items: left;
  }
  
  .image-placeholder {
    background-image: url(/src/assets/Mask.png);
    width: 100%;
    height: 50px;
  }
  
  h1, h2, p {
    margin: 0;
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
  