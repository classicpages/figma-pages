
<template>
    <div class="section-two">
      <!-- Section Content -->
      <div class="section-content">
        <div class="free">Free Sample</div>
        <div>
          <h2 class="Powerful">Powerful Generator and Free <br> Figma Sources</h2>
          <p class="start">Startup Framework contains components and complex blocks which can easily be <br> integrated into almost any design. All of the components are made in the same style, 
            and <br> can easily be integrated into projects, allowing you to create hundreds of solutions.</p>
        </div>
      
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
    height: 540px;
    min-height: 100vh;
    position: relative;
    max-width: 100%;
    background-color: blue; /* Fallback background color */
  }
  
  .section-content {
    margin-top: 6rem;
  }
  
  .free{
    font-size: 19px;
    margin-bottom: 0.5rem;
    font-weight: 400;
  }
  
  .Powerful{
    font-size: 45px;
    margin-bottom: 1rem;
    font-weight: 600;
  }
  
  .start{
    font-size: 16px;
    margin-bottom: 2rem;
    font-weight: 200;
    max-width: 7505px;
  }
  
  /* Responsive Styles */
  @media (max-width: 768px) {
    .free {
      font-size: 16px;
    }   
  
    .Powerful{
      font-size: 25 px;
    }
  
    .start{
      font-size: 1rem;
    }

  }
  </style>
  

























  