<template>
    <section class="section-seven">
      <div class="header">
        <h1>Last works</h1>
        <button class="view-all-work">View all work</button>
      </div>
      <div class="works-container">
        <div class="work-item">
          <div class="work-image"></div>
          <div class="work-text">
            <span>UI kit</span>
            <span>Mozart Project</span>
          </div>
        </div>
        <div class="work-item">
          <div class="work-image"></div>
          <div class="work-text">
            <span>UI kit</span>
            <span>Mozart Project</span>
          </div>
        </div>
        <div class="work-item">
          <div class="work-image"></div>
          <div class="work-text">
            <span>UI kit</span>
            <span>Mozart Project</span>
          </div>
        </div>
        <div class="work-item">
          <div class="work-image"></div>
          <div class="work-text">
            <span>UI kit</span>
            <span>Mozart Project</span>
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
  }
  
  .view-all-work {
    background-color: white;
    color: blue;
    border: none;
    padding: 10px 20px;
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
    border: 2px solid white;
    padding: 20px;
    flex: 1 1 calc(50% - 20px);
    box-sizing: border-box;
    text-align: left;
  }
  
  .work-image {
    background-image: url('@/assets/4c269f57807850115899b4611a2bf3ba.jpeg');
    background-size: cover;
    background-position: center;
    height: 200px;
    margin-bottom: 10px;
  }
  
  .work-text {
    display: flex;
    justify-content: space-between;
  }
  
  .work-text span {
    display: inline-block;
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
  