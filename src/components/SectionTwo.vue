
<template>
    <div class="section-two">
      <!-- Section Content -->
      <div class="section-content">
        <h1 class="free">Free Sample</h1>
        <h2 class="Powerful">Powerful Generator and Free Figma Sources</h2>
        <p class="start">Startup Framework contains components and complex blocks which can easily be integrated into almost any design. All of the components are made in the same style, and can easily be integrated into projects, allowing you to create hundreds of solutions.</p>
      </div>
    </div>
  </template>

  
  <script>
  export default {
    name: 'SectionTwo'
  }
  </script>
  
  
  <style scoped>
  .section-two {
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
  
  .section-content {
    margin-top: 6rem;
  }
  
  .free{
    font-size: 14px;
    margin-bottom: 0.5rem;
    font-weight: 300;
  }
  
  .Powerful{
    font-size: 35px;
    margin-bottom: 1rem;
    font-weight: 600;
  }
  
  .start{
    font-size: 13.5px;
    margin-bottom: 2rem;
    font-weight: 200;
  }
  
  /* Responsive Styles */
  @media (max-width: 768px) {
    .free {
      font-size: 16px;
    }
  
    .Powerful{
      font-size: 25px;
    }
  
    .start{
      font-size: 1rem;
    }
  }
  </style>
  

























  