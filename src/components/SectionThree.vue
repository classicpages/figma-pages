<template>
  <div class="section-three">
    <div class="laptop">
      <div class="we">
        <img class="left-image" src="/src/assets/Mockup.png" alt="Left Image" />
      </div>

      <div class="create">
        <div class="all">
          <div class="something">
            <h2 class="short">We Create Something New</h2>
          </div>
          <div class="new">
            <p>
              We have created a new product that will help designers,
              developers, and companies create websites for their startups
              quickly and easily.
            </p>
          </div>
        </div>

        <div class="icons">
          <div class="text" style="margin-right: 29px;">
            <div>
              <img src="/src/assets/fa-commenting-o.png" alt="" />
            </div>
            <div class="text">30 New feature pages</div>
            <p>
              Startup Framework contains the components and complex blocks which
              can easily be read.
            </p>
          </div>

          <div class="text">
            <div>
              <img src="/src/assets/fa-commenting-o (1).png" alt="" />
            </div>
            <div class="text">Useful Symbol Components</div>
            <p>
              Samples will show you the feeling on how to play around using
              the components.
            </p>
          </div>
        </div>

        <!-- Dots Indicator -->
        <div class="dots-container">
          <span class="dot active"></span>
          <span class="dot"></span>
          <span class="dot"></span>
          <span class="dot"></span>
          <span class="dot"></span>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "SectionThree",
};
</script>
<style scoped>
@import url('https://fonts.googleapis.com/css2?family=DM+Sans:ital,opsz,wght@0,9..40,100..1000;1,9..40,100..1000&display=swap');

.section-three {
  position: relative; /* Added to ensure children can use absolute positioning */
  background-image: url("/src/assets/Rectangle.png");
  background-size: cover;
  background-position: center;
  background-repeat: no-repeat;
  max-height: 736px;
  max-width: 100%;
  background-color: #2f1893;
  padding-top: 100px;
  padding-bottom: 100px;
  color: white;
  font-family: 'DM Sans', sans-serif;
}

.laptop {
  max-height: 535px;
}

.all {
  margin-bottom: 65.5px;
}

.icons {
  margin-right: 29px;
}

.text {
  display: inline-block;
  max-width: 271px;
  max-height: 186.8px;
  top: 391.6px;
  left: 515px;
  gap: 0px;
  opacity: 0px;
  margin-top: 27px;
  line-height: 26px;
}

.we {
  height: 100%;
  margin-right: 33.45px;
  display: inline-block;
}

.create {
  padding-top: 58px;
  display: inline-block;
}

.short {
  font-size: 40px;
  font-weight: 600;
  font-size: 42px;
  line-height: 52px;
  text-align: left;
  width: 532px;
  height: 52px;
}

.something {
  width: 532px;
  height: 52px;
}

.new {
  font-size: 22px;
  width: 600px;
  height: 96px;
  font-weight: 300;
  text-align: left;
}

.dots-container {
  position: absolute; /* Positioned absolutely relative to .section-three */
  right: 20px; /* Distance from the right edge of the section */
  top: 50%; /* Vertically centered in the section */
  transform: translateY(-50%); /* Adjust vertical alignment */
  display: flex;
  flex-direction: column;
  align-items: center;
  margin-right: 60px;
}

.dot {
  width: 10px;
  height: 10px;
  border-radius: 50%;
  display: block;
  background-color: rgb(173, 163, 163);
  margin-bottom: 10px; /* Space between the dots */
}

.dot.active {
  background-color: white;
}

/* Responsive Styles */

@media (max-width: 1440px) {
  .text {
    max-width: 250px;
    max-height: 180px;
  }
  .short {
    font-size: 38px;
    width: 500px;
  }
  .new {
    width: 550px;
  }
}

@media (max-width: 1200px) {
  .text {
    max-width: 220px;
    max-height: 170px;
  }
  .short {
    font-size: 36px;
    width: 450px;
  }
  .new {
    width: 500px;
  }
}

@media (max-width: 1024px) {
  .text {
    max-width: 200px;
    max-height: 150px;
  }
  .short {
    font-size: 34px;
    width: 400px;
  }
  .new {
    width: 450px;
  }
}

@media (max-width: 1000px) {
  .text {
    max-width: 180px;
    max-height: 140px;
  }
  .short {
    font-size: 32px;
    width: 350px;
  }
  .new {
    width: 400px;
  }
}

@media (max-width: 900px) {
  .text {
    max-width: 160px;
    max-height: 130px;
  }
  .short {
    font-size: 30px;
    width: 300px;
  }
  .new {
    width: 350px;
  }
}

@media (max-width: 810px) {
  .text {
    max-width: 140px;
    max-height: 120px;
  }
  .short {
    font-size: 28px;
    width: 270px;
  }
  .new {
    width: 320px;
  }
}

@media (max-width: 768px) {
  .text {
    max-width: 80px;
    max-height: 100px;
  }
  .short {
    font-size: 32px;
    width: 200px;
  }
  .new {
    width: 200px;
  }
  .dots-container {
    right: 10px; 
  }
}

@media (max-width: 480px) {
  .text {
    max-width: 110px;
    max-height: 110px;
  }
  .short {
    font-size: 30px;
    width: 330px;
  }
  .new {
    width: 310px;
  }
}
</style>
