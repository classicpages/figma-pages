
<template>
    <div class="section-three">
      <!-- Background Image -->
      <div class="background"></div>
      
      <!-- Section Content -->
      <div class="section-content">
        <h1>We Create Something New</h1>
        <h2>We have created a new product that will help designers, developers, and companies create websites for their startups quickly and easily.</h2>
        
        <!-- Flexbox Layout for Additional Text -->
        <div class="flex-container">
          <p>30 New feature pages, Startup Framework contains components and complex blocks which can easily.</p>
          <p>Useful Symbol Components, Samples will show you the feeling on how to play around using the components.</p>
        </div>
      </div>
      
      <!-- Left Side Image -->
    
    </div>
  </template>
  

  <script>
  export default {
    name: 'SectionThree'
  }
  </script>
  
  
  <style scoped>
  .section-three {
    background-image: url('/public/Image.png');
    background-size: cover;
    background-position: center;
    background-repeat: no-repeat;
    color: white;
    text-align: center;
    padding: 2rem;
    display: flex;
    flex-direction: column;
    justify-content: center;
    min-height: 100vh;
    position: relative;
    background-color: blue; /* Fallback background color */
  }
  
  .background {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background-image: url('/public/Image.png');
    background-size: cover;
    background-position: center;
    background-repeat: no-repeat;
    z-index: -1;
  }
  
  .section-content {
    margin-top: 2rem;
  }
  
  .section-content h1 {
    font-size: 3rem;
    margin-bottom: 0.5rem;
  }
  
  .section-content h2 {
    font-size: 2rem;
    margin-bottom: 1rem;
  }
  
  .flex-container {
    display: flex;
    justify-content: space-around;
    flex-wrap: wrap;
    margin-top: 2rem;
  }
  
  .flex-container p {
    flex: 1;
    margin: 1rem;
    font-size: 1.2rem;
  }
  
  .left-image {
    position: absolute;
    top: 50%;
    left: 2rem;
    transform: translateY(-50%);
  }
  
  .left-image img {
    max-width: 100%;
    height: auto;
    display: block;
  }
  
  /* Responsive Styles */
  @media (max-width: 768px) {
    .section-content h1 {
      font-size: 2.5rem;
    }
  
    .section-content h2 {
      font-size: 1.8rem;
    }
  
    .flex-container {
      flex-direction: column;
    }
  
    .flex-container p {
      font-size: 1rem;
      margin: 0.5rem;
    }
  
    .left-image {
      position: relative;
      top: auto;
      left: auto;
      transform: none;
      margin: 1rem auto;
    }
  
    .left-image img {
      width: 80%;
      margin: 0 auto;
    }
  }
  </style>
  




















































