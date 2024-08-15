<template>
  <section class="section-five">
    <h1>Our Happy Clients</h1>
    <div class="good-morning-container">
      <div class="good-morning">
        <div class="imgs">
          <img src="/src/assets/Mask (3).png">
        </div>
        <div class="text-container">
         <div class="text">Get a fully retina-ready site when you build with Startup Framework. Websites look sharper and
          more gorgeous on devices with retina display support.
          <p class="txt">Rayhan Curran</p></div>
        </div>
      </div>
      <div class="good-morning">
        <div class="imgs">
          <img src="/src/assets/Mask (1).png">
        </div>
        <div class="text-container">
          <div class="text">As a business targeting high net worth individuals,
            we were looking for a slick, cool, and minimalistic design for our website
            <p class="txtK">Kayley Frame</p></div>
        </div>
      </div>
    </div>
    <div class="good-morning-container">
      <div class="good-mornings">
        <div class="imgs">
          <img src="/src/assets/Mask (2).png">
        </div>
        <div class="text-container">
          <div class="text"> The most important part of the Startup Framework is the samples
            <p class="txtG">Gene Whitfield</p></div>
        </div>
      </div>
      <div class="good-mornings">
        <div class="imgs">
          <img src="/src/assets/Mask (3).png">
        </div>
        <div class="text-container">
          <div class="text">I’ve built my website with Startup just in one day,
            and it was ready-to-go.
            <p class="txtA">Allan Kim</p></div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: 'SectionFive'
}
</script>

<style scoped>
.section-five {
  background-color: #1E0E62;
  color: white;
  padding: 20px;
  display: flex;
  flex-direction: column;
  max-height: 100vh;
  position: relative;
  align-items: center;
  max-width: 100%;
}

h1 {
  margin-bottom: 40px;
  font-size: 26px;
  font-weight: 700;
  text-align: left;
  margin-right: 450px;
}

.good-morning-container {
  display: flex;
  width: 50%;
  justify-content: space-between;
  flex-wrap: wrap;
  align-items: center;
  height: 260px;
}

.good-morning, .good-mornings {
  background-color: #1E0E62;
  color: white;
  padding: 19px;
  max-width: 50%;
  box-sizing: border-box;
  display: flex;
  align-items: center;
  border: 1px solid gray;
  border-radius: 10px;
  margin-bottom: 10px;
}

.imgs {
  flex-shrink: 0;
  margin-right: 20px;
  margin-bottom: 140px;
  width: 60px;
  height: 60px;
  border-radius: 10px 0px 0px 0px;
}

.imgs img {
  width: 60px;
  height: 60px;
  border-radius: 1px;
}

.text-container {
  flex-grow: 1;
  font-size: 18px;
  font-weight: 500;  
}

.txt {
  color: rgb(148, 146, 146);
  margin-top: 30px;
}

.txtK {
  margin-top: 52px;
  color: rgb(148, 146, 146);
}

.text {
  text-align: left;
  width: 200px;
  height: 170px;
  }

.txtG {
  color: rgb(148, 146, 146);
  margin-top: 50px;
}

.txtA {
  color: rgb(148, 146, 146);
  margin-top: 45px;
}

@media (max-width: 768px) {
  .good-morning, .good-mornings {
    flex: 1 1 100%;
    margin-bottom: 15px;
  }
  
  .imgs {
    margin-bottom: 10px;
    margin-right: 15px;
  }

  .text-container {
    text-align: left;
  }
}

@media (max-width: 480px) {
  .good-morning, .good-mornings {
    flex: 1 1 100%;
    flex-direction: column;
    align-items: flex-start;
    text-align: left;
  }

  .imgs {
    margin-bottom: 15px;
    margin-right: 0;
  }
}
</style>
