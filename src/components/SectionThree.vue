<template>
  <div class="section-three">
    <!-- Section Content -->
    <div class="section-content">
      <div>
        <h2 class="Powerful">We Create Something New</h2>
        <p class="start">
          We have created a new product that will help designers, developers, and companies create websites for their startups quickly and easily.
        </p>
      </div>
    </div>

    <!-- Flex Container for the Second Div -->
    <div class="section-extra">
      <img class="left-image" src="/src/assets/Mockup.png" alt="Left Image">
      <div class="icons-text">
        <div class="icon-text-item">
          <div class="icon"><img src="/src/assets/fa-commenting-o.png" alt=""></div>
          <div class="text">30 New feature pages</div>
          <p class="frame">Startup Framework contains components and complex blocks which can easily.</p>
        </div>
        <div class="icon-text-item">
          <div class="icon"><img src="/src/assets/fa-commenting-o (1).png" alt=""></div>
          <div class="text">Useful Symbol Components</div>
          <p class="frame">Samples will show you the feeling on how to play around using the components.</p>
        </div>
      </div>
      <div class="dots-container">
        <span class="dot active"></span>
        <span class="dot"></span>
        <span class="dot"></span>
        <span class="dot"></span>
        <span class="dot"></span>
      </div>
    </div>
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
  text-align: center;
  color: white;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  max-height: 736px;
  position: relative;
  max-width: 100%;  
  background-color: #2F1893;
  padding-top: 100px;
  padding-bottom: 100px;
}

/* Adjust the second div to display flex */
.section-extra {
  display: flex;
  align-items: center;
  justify-content: space-between;
  width: 100%;
}

.section-content {
  max-width: 100%;  
  max-height: 80px;
  text-align: center;
  margin-left: 350px;
}

.left-image {
  max-width: 500px;
  width: 733.6px;
  height: 449.88px;
  top: 126.41px;
  left: -376.89px;
  border-radius: 11px;
}

.icons-text {
display: flex;
justify-content: space-around;
flex-grow: 1;
margin-left: 65.6px;
}

.icon-text-item {
  display: flex;
  flex-direction: column;
  align-items: center;
  margin-right: 30px;
}

.icon {
  font-size: 24px;
  margin-bottom: 0.5rem;
  float: left;
}

.frame {
  font-size: 16px;
  font-weight: 300;
  height: 78px;
  width: 270px;
  text-align: left;
}

.text {
  font-size: 17px;
  height: 26px;
  text-align: left;
}

.Powerful {
  font-size: 40px;
  font-weight: 600;
  height: 30px;
  text-align: center;
}

.start {
  font-size: 17px;
  width: 600px;
  height: 96px;
  margin-bottom: 33px;
  margin-left: 10%;
  font-weight: 300;
  text-align:left;
}

.dots-container {
  display: flex;
  flex-direction: column;
  align-items: center;
  margin-left: 2rem;
  margin-bottom: 120px;
}

.dot {
  width: 10px;
  height: 10px;
  margin: 5px 0;
  border-radius: 50%;
  display: inline-block;
  background-color: rgb(153, 146, 146);
  margin-right: 60px;
}

.dot.active {
  background-color: white;
}

/* Responsive Styles */
@media (max-width: 768px) {
  .free {
    font-size: 16px;
  }   

  .Powerful {
    font-size: 25px;
  }

  .start {
    font-size: 1rem;
  }

  .section-extra {
    flex-direction: column;
    align-items: center;
    margin: 0;
  }

  .left-image {
    margin: 1rem 0;
  }

  .icon-text-item {
    margin-bottom: 1rem;
  }

  .icons-text {
    margin-left: 0;
  }

  .dots-container {
    margin: 1rem 0;
  }
}
</style>
