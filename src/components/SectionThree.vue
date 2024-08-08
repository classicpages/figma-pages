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
          <p class="new"><img class="icon" src="/src/assets/fa-commenting-o (1).png"> 30 NEW FEATURE PAGES</p>
          <p class="new">Startup Framework contains components and complex blocks which can easily</p>


          <p class="use"> <img class="icon" src="/src/assets/fa-commenting-o.png"> USEFUL SYMBOL COMPONENTS</p> 
          <p class="use">Samples will show you the feeling on how to play around using the components.</p>
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
    background-image: url('/src/assets/Rectangle.png');
    background-size: cover;
    background-position: center;
    background-repeat: no-repeat;
    color: white;
    text-align: left;
    padding: 2rem;
    display: flex;
    flex-direction: column;
    justify-content: left;
    min-height: 100vh;
    position: relative; 
  }
  
  .background {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background-image: url();
    background-size: cover;
    background-position: center;
    background-repeat: no-repeat;
    z-index: -1;
  }
  
  .section-content {
    margin-top: 2rem;
  }
  
  .section-content h1 {
    font-size: 24px;
    margin-bottom: 0.5rem;
  }
  
  .section-content h2 {
    font-size: 15px;
    margin-bottom: 1rem;
  }
  
  .flex-container {
    display: flex;
    align-items: center;
    justify-content: center;
    margin-top: 2rem;
  }
  
  .new{
    margin: 10px;
    font-size: 15px;
  }

  .icon {
    width: 30px;
    height: 30px;
  }

  .use{
    margin: 10px;
    font-size: 15px;
    

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
      font-size: 19px;
    }
  
    .section-content h2 {
      font-size: 15px;
    }
  
    .flex-container {
      flex-direction: column;
    }
  
    .new{
      font-size: 1rem;
      margin: 0.5rem;
    }

    .use{
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
  