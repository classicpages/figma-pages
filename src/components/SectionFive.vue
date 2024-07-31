<template>
    <section class="section-five">
      <h1>Our Happy Clients</h1>
      <div class="good-morning-container">
        <div class="good-morning">Get a fully retina ready site when you build with Startup Framework. Websites look sharper and more gorgeous on devices with retina display support</div>
        <div class="good-morning">As a business targeting high net worth individuals, we were looking for a slick, cool and mini-malistic design for our website</div>
      </div>
      <div class="good-morning-container">
        <div class="good-mornings">The most important part of the Startup Framework is the samples</div>
        <div class="good-mornings">I’ve built my website with Startup just in one day, and it was ready-to-go. </div>
      </div>
    </section>
  </template>
  
  <script>
  export default {
    name: 'SectionFive'
  }
  </script>
  
  <style scoped>
  .section-five {
    background-color: #1E0E62;
    color: white;
    padding: 20px;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
  }
  
  h1 {
    margin-bottom: 20px;
  }
  
  .good-morning-container {
    display: flex;
    gap: 20px;
    width: 100%;
    justify-content: space-between;
  }
  
  .good-morning {
    background-color: #1E0E62;
    color: white;
    padding: 20px;
    flex: 1 1 calc(50% - 20px);
    box-sizing: border-box;
    text-align: center;
    border: 2px solid white;
  }
  
  .good-mornings {
    background-color: #1E0E62;
    color: white;
    padding: 20px;
    flex: 1 1 calc(50% - 20px);
    box-sizing: border-box;
    text-align: center;
    border: 2px solid white;
    margin-top: 15px;
  }



  @media (max-width: 768px) {
    .good-morning {
      flex: 1 1 100%;
    }
  }
  
  @media (max-width: 480px) {
    .good-morning {
      flex: 1 1 100%;
    }
  }
  </style>
  