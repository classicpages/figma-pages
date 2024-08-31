<template>
  <section class="section-seven">
    <div class="header">
      <h1>Last works</h1>
      <button class="view-all-work">View all works</button>
    </div>
    <div class="works-container">
      <div class="work-item">
        <div class="work-image">
          <img src="/src/assets/Work 1.png" alt="" />
        </div>
        <div class="work-text"></div>
      </div>
      <div class="work-item">
        <div class="work-image">
          <img src="/src/assets/Work 2.png" alt="" />
        </div>
        <div class="work-text"></div>
      </div>
      <div class="work-item">
        <div class="work-image">
          <img src="/src/assets/Work 3.png" alt="" />
        </div>
        <div class="work-text"></div>
      </div>
      <div class="work-item">
        <div class="work-image">
          <img src="/src/assets/Work 4.png" alt="" />
        </div>
        <div class="work-text"></div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "SectionSeven",
};
</script>

<style scoped>
@import url("https://fonts.googleapis.com/css2?family=DM+Sans:ital,opsz,wght@0,9..40,100..1000;1,9..40,100..1000&display=swap");

.section-seven {
  background-color: blue;
  color: white;
  padding: 30px;
  max-width: 100%;
}

.header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-bottom: 20px;
  flex-wrap: wrap;
}

h1 {
  margin: 0;
  font-weight: 700;
  margin-left: 200px;
  width: 213px;
  height: 52px;
  margin-top: 100px;
  font-family: 'DM Sans', sans-serif;
  font-size: 42px;
  line-height: 52px;
  letter-spacing: -0.4px;
  text-align: left;
}

.view-all-work {
  background-color: blue;
  color: white;
  border: 1px solid rgb(236, 232, 232);
  padding: 10px 20px;
  border-radius: 17px;
  font-size: 12px;
  cursor: pointer;
  margin-right: 100px;
  margin-top: 100px;
}

.view-all-work:hover {
  background-color: lightblue;
}

.works-container {
  display: flex;
  flex-wrap: wrap;
  gap: 20px;
  margin-top: 50px;
}

.work-item {
  background-color: blue;
  padding: 10px;
  box-sizing: border-box;
  text-align: left;
  border-radius: 10px;
  transition: transform 0.3s ease;
}

.work-item:hover {
  transform: scale(1.05);
}

.work-image img {
  width: 100%;
  border-radius: 10px;
}

.work-text {
  text-align: center;
  font-size: 15px;
  margin-top: 10px;
}

.work-text span {
  display: block;
}

/* Responsive Styles */
@media (max-width: 1440px) {
  h1 {
    font-size: 38px;
  }
  .view-all-work {
    font-size: 14px;
  }
}

@media (max-width: 1200px) {
  h1 {
    font-size: 34px;
    margin-left: 150px;
  }
  .view-all-work {
    font-size: 14px;
    margin-right: 50px;
  }
}

@media (max-width: 1024px) {
  h1 {
    font-size: 30px;
    margin-left: 100px;
  }
  .view-all-work {
    font-size: 14px;
    margin-right: 30px;
  }
}

@media (max-width: 1000px) {
  h1 {
    font-size: 28px;
    margin-left: 80px;
  }
  .view-all-work {
    font-size: 13px;
    margin-right: 20px;
  }
}

@media (max-width: 900px) {
  h1 {
    font-size: 26px;
    margin-left: 50px;
  }
  .view-all-work {
    font-size: 13px;
    margin-right: 10px;
  }
}

@media (max-width: 810px) {
  h1 {
    font-size: 24px;
    margin-left: 30px;
  }
  .view-all-work {
    font-size: 12px;
    margin-right: 5px;
  }
}

@media (max-width: 768px) {
  .work-item {
    flex: 1 1 calc(50% - 20px);
  }
  h1 {
    font-size: 22px;
    margin-left: 20px;
  }
  .view-all-work {
    font-size: 12px;
    width: 100%;
    text-align: center;
    padding: 12px 0;
    margin-top: 10px;
  }
  .header {
    justify-content: center;
  }
}

@media (max-width: 480px) {
  .work-item {
    flex: 1 1 100%;
  }
  h1 {
    font-size: 18px;
    margin: 0 auto;
  }
  .view-all-work {
    font-size: 12px;
    width: 100%;
    text-align: center;
    padding: 12px 0;
    margin-top: 10px;
  }
  .header {
    flex-direction: column;
    align-items: center;
  }
  .works-container {
    margin-left: 0;
  }
}
</style>
