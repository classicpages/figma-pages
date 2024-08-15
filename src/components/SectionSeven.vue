<template>
  <section class="section-seven">
    <div class="header">
      <h1>Last works</h1>
      <button class="view-all-work">View all works</button>
    </div>
    <div class="works-container">
      <div class="work-item">
        <div class="work-image">
          <img src="/src/assets/Work 1.png" alt="">
        </div>
        <div class="work-text">
        </div>
      </div>
      <div class="work-item">
        <div class="work-image">
          <img src="/src/assets/Work 2.png" alt="">
        </div>
        <div class="work-text">
        </div>
      </div>
      <div class="work-item">
        <div class="work-image">
          <img src="/src/assets/Work 3.png" alt="">
        </div>
        <div class="work-text">
        </div>
      </div>
      <div class="work-item">
        <div class="work-image">
          <img src="/src/assets/Work 4.png" alt="">
        </div>
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
  font-size: 22px;
}

.view-all-work {
  background-color: blue;
  color: white;
  border: 1px solid rgb(236, 232, 232);
  padding: 10px 20px;
  border-radius: 17px;
  font-size: 12px;
  cursor: pointer;
}

.view-all-work:hover {
  background-color: lightblue;
}

.works-container {
  display: flex;
  flex-wrap: wrap;
  max-height: 816px;
  width: 100%;
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

@media (max-width: 768px) {
  .work-item {
    flex: 1 1 calc(50% - 20px);
  }
}

@media (max-width: 480px) {
  .work-item {
    flex: 1 1 100%;
  }

  .view-all-work {
    width: 100%;
    text-align: center;
    padding: 12px 0;
    margin-top: 10px;
  }

  .header {
    justify-content: center;
  }

  h1 {
    font-size: 18px;
  }
}
</style>
