<template>
    <section class="section-seven">
      <div class="header">
        <h1>Last works</h1>
        <button class="view-all-work">View all works</button>
      </div>
      <div class="works-container">
        <div class="work-item">
          <div class="work-image"><img src="/src/assets/Work 1.png" alt=""></div>
          <div class="work-text">
           
          </div>
        </div>
        <div class="work-item">
          <div class="work-image"><img src="/src/assets/Work 2.png" alt=""></div>
          <div class="work-text">
          </div>
        </div>
        <div class="work-item">
          <div class="work-image"><img src="/src/assets/Work 3.png" alt=""></div>
          <div class="work-text">
          </div>
        </div>
        <div class="work-item">
          <div class="work-image"><img src="/src/assets/Work 4.png" alt=""></div>
          <div class="work-text">
          </div>
        </div>
      </div>
    </section>
  </template>
  <script>
  export default {
    name: 'SectionSeven'
  }
  </script>
  
  <style scoped>
  .section-seven {
    background-color: blue;
    color: white;
    padding: 20px;
  }
  
  .header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin-bottom: 20px;
  }
  
  h1 {
    margin: 0;
    font-weight: 700;
    font-size: 22px;
  }
  
  .view-all-work {
    background-color: blue;
    color: white;
    border: 1px solid rgb(236, 232, 232);
    padding: 10px 20px;
    border-radius: 17px;
    font-size: 10px;
    cursor: pointer;
  }
  
  .view-all-work:hover {
    background-color: lightblue;
  }
  
  .works-container {
    display: flex;
    flex-wrap: wrap;
    gap: 20px;
  }
  
  .work-item {
    background-color: blue;
    padding: 20px;
    flex: 1 1 calc(50% - 20px);
    box-sizing: border-box;
    text-align: left;
  }
  
  .work-image {
    
    border-radius: 5px;
    margin-bottom: 10px;
  }
  
  .work-text {
    display:block;
    justify-content: space-between;
    text-align: center;
    font-size: 15px;
  }
  
  .work-text span {
    display: block;
  }
  
  @media (max-width: 768px) {
    .work-item {
      flex: 1 1 100%;
    }
  }
  
  @media (max-width: 480px) {
    .work-image {
      height: 150px;
    }
  
    .view-all-work {
      padding: 8px 16px;
    }
  }
  </style>
  