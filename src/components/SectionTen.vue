<template>
    <div class="section-ten">
      <div class="content-wrapper">
        <h1>Plans & Pricing</h1>
        <p>Startup Framework is free forever - you only pay for <br> custom domain hosting or to export your site.</p>
        <div class="plans-container">
          <div class="plan starter">
            <h2>Starter</h2>
            <p class="price">9.99</p>
            <p class="details">2GB of Space <br> 14 days backups<br> Social integration<br> Client billing <br>
              2GB of Space <br> 14 days backups<br> Social integration<br> Client billing.</p>
            <button class="get-started">Get Started</button>
          </div>
          <div class="plan professional">
            <h2>Professional</h2>
            <p class="price">19.99</p>
            <p class="details">2GB of Space <br> 14 days backups<br> Social integration<br> Client billing <br>
              2GB of Space <br> 14 days backups<br> Social integration<br> Client billing.</p>
            <button class="get-started red">Get Started</button>
          </div>
          <div class="plan team">
            <h2>Team</h2>
            <p class="price">49.99</p>
            <p class="details">2GB of Space <br> 14 days backups<br> Social integration<br> Client billing <br>
              2GB of Space <br> 14 days backups<br> Social integration<br> Client billing.</p>
            <button class="get-started">Get Started</button>
          </div>
        </div>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    name: "SectionTen"
  };
  </script>
  
  <style scoped>
  .section-ten {
    text-align: center;
    padding: 20px;
    background-image: url('/src/assets/Mask.png'); /* Add your background image URL here */
    background-size: cover;
    background-position: center;
  }
  
  .content-wrapper {
    max-width: 1200px;
    margin: 0 auto;
    padding: 20px;
    color: #fff;

  }
  
  .plans-container {
    display: flex;
    justify-content: space-around;
    gap: 20px;
  }
  
  .plan {
    min-width: 250px;
    border: 1px solid grey;
    padding: 20px;
    box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
    display: block;
    color: #fff;

  }
  
  .plan h2 {
    margin: 0 0 10px;
    color: #fff;
    font-size: 15px;
    font-weight: 500; 
  }
  
  .plan .price {
    font-size: 45px;
    margin: 0 0 10px;
    color: #fff;

  }
  
  .plan .details {
    display: block;
    margin: 40px;
    color: #fff;
    font-weight: 500;
    font-size: 15px;
  }

  
  .get-started {
    padding: 10px 20px;
    border: none;
    color: white;
    background-color: rgb(47, 80, 94);
    border-radius: 20px;
    cursor: pointer;
  }
  
  .get-started.red {
    background-color: #E93A7D;
  }
  
  @media (max-width: 768px) {
    .plans-container {
      flex-direction: column;
      align-items: center;
    }
  }
  </style>
