<template>
    <section class="section-six">
      <div class="content">
        <h1>Easy to setup. <br> Easy to maintain</h1>
        <p>Bootstrap is a widely-used, sleek, intuitive and <br> powerful front-end framework for faster and <br> easier web development.</p>
        <button class="get-started-button">Get Started</button>
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
    padding: 40px;
    display: flex;
    justify-content: center;
    align-items: center;
    min-height: 100vh;
    position: relative;
    max-width: 100%;
    text-align: center;
    background-color: #2F1893;
  }
  
  .content {
    max-width: 800px;
    width: 100%;
  }
  
  h1 {
    font-size: 35px;
    margin-bottom: 20px;
    font-weight: 500;
  }
  
  p {
    font-size: 15px;
    margin-bottom: 40px;
  }
  
  .get-started-button {
    background-color:  #25DAC5;
    color: white;
    border: none;
    border-radius:22px;
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
  