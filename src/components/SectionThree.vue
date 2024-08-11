<template>
  <div class="section-three">
    <!-- Section Content -->
    <div class="section-content">
      <div>
        <h2 class="Powerful">We Create Something New</h2>
        <p class="start">We have created a new product that will help designers,<br>
           developers and companies create websites for their <br> startups quickly and easily..</p>
      </div>
    </div>

    <!-- Flex Container for the Second Div -->
    <div class="section-extra">
      <img class="left-image" src="/src/assets/Screen Effects.png" alt="Left Image">
      <div class="icons-text">
        <div class="icon-text-item">
          <div class="icon"><img src="/src/assets/fa-commenting-o.png" alt=""></div> 
          <div class="text">30 New feature pages</div>
          <p class="frame">Startup Framework contains components and complex blocks which can easily. </p>
        </div>
        <div class="icon-text-item">
          <div class="icon"><img src="/src/assets/fa-commenting-o (1).png" alt=""></div>
          <div class="text">Useful Symbol Components</div>
          <p class="frame">Samples will show you the feeling on how to play around using the components.</p>
        </div>
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
  min-height: 100vh;
  position: relative;
  max-width: 100%;  
 background-color: rgb(118, 118, 180);
}

/* Adjust the second div to display flex */
.section-extra {
  display: flex;
  align-items: center;
  justify-content: space-between;
  width: 100%;
  margin-top: 2rem;
}

.left-image {
  max-width: 200px;
  align-items: start;
  float: left;
  margin-bottom: 50px;
}

.icons-text {
  display: flex;
  justify-content: space-around;
  flex-grow: 1;
}

.icon-text-item {
  display: flex;
  flex-direction: column;
  align-items: center;
  margin: 0 1rem;
}

.icon {
  font-size: 24px;
  margin-bottom: 0.5rem;
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

.free {
  font-size: 14px;
  margin-bottom: 0.5rem;
  font-weight: 300;
}

.Powerful {
  font-size: 40px;
  margin-bottom: 10px;
  margin-top: 30px;
  font-weight: 600;
  height: 50px;
  text-align: left;
}

.start {
  font-size: 17px;
  width: 600px;
  height: 96px;
  margin-bottom: 2rem;
  font-weight: 200;
  font-weight: 300;
  text-align: left;
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
  }

  .left-image {
    margin-right: 0;
    margin-bottom: 1rem;
  }

  .icon-text-item {
    margin-bottom: 1rem;
  }
}
</style>
