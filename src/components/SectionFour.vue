<template>
  <div class="section-four">
    <div class="text-section">
      <h1 class="text">
        We solve digital problems with an outstanding creative flare
      </h1>
      <p class="we">
        We have created a new product that will help designers,
        developers, and companies create websites for their startups
        quickly and easily.
      </p>
    </div>

    <div class="form-section">
      <div class="tab-container">
        <button
          :class="['tablinks', { active: showSignUp }]"
          @click="toggleForm(true)"
        >
          Sign Up
        </button>
        <button
          :class="['tablinks', { active: !showSignUp }]"
          @click="toggleForm(false)"
        >
          Login
        </button>
      </div>

      <div class="sign-up-form" v-show="showSignUp">
        <input type="email" placeholder="Your email" />
        <input type="password" placeholder="Your password" />
        <button>Create an Account</button>
        <div class="or-line">
          <div class="line"></div>
          <span>or</span>
          <div class="line"></div>
        </div>
        <button class="twitter-button">Login via Twitter</button>
      </div>

      <div class="login-form" v-show="!showSignUp">
        <input type="email" placeholder="Your email" />
        <input type="password" placeholder="Your password" />
        <button>Login</button>
        <div class="or-line">
          <div class="line"></div>
          <span>or</span>
          <div class="line"></div>
        </div>
        <button class="twitter-button">Login via Twitter</button>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      showSignUp: true,
    };
  },
  methods: {
    toggleForm(showSignUp) {
      this.showSignUp = showSignUp;
    },
  },
};
</script>
<style scoped>
@import url("https://fonts.googleapis.com/css2?family=DM+Sans:ital,opsz,wght@0,9..40,100..1000;1,9..40,100..1000&display=swap");

.section-four {
  display: flex;
  justify-content: space-between;
  align-items: center;
  background-image: url("/public/Image.png");
  background-size: cover;
  color: white;
  flex-wrap: wrap;
  height: 750px;
  position: relative;
  max-width: 1400px;
  background-color: #2f1893;
  font-family: "DM Sans", sans-serif;
  padding: 20px;
}

.text-section {
  flex: 1;
  padding: 20px;
}

.text {
  font-size: 42px;
  line-height: 52px;
  letter-spacing: -0.4px;
  text-align: left;
  margin-bottom: 32px;
}

.we {
  font-size: 16px;
  line-height: 26px;
  text-align: left;
}

.form-section {
  background: white;
  color: black;
  box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
  width: 470px;
  height: 550px;
  padding: 20px;
  margin: 20px;
}

.tab-container {
  display: flex; 
  justify-content: space-between;
  align-items: center;
  margin-bottom: 20px;
}

.tablinks {
  flex: 1;
  cursor: pointer;
  text-align: center;
  background-color: #f1f1f1;
  outline: none;
  color: #000;
  border-bottom: 2px solid transparent;
}

.tablinks.active {
  border-bottom: 2px solid black;
  font-weight: bold;
  background-color: white;
}

input {
  width: 330px;
  height: 50px;
  border-radius: 50px;
  border: 2px solid #ccc;
  margin: 10px 0;
  padding-left: 20px; 
}

button {
  width: 330px;
  height: 50px;
  border-radius: 50px;
  border: none;
  background: #25dac5;
  color: white;
  cursor: pointer;
  margin: 10px 0;
}

.twitter-button {
  background: #1da1f2;
}

.or-line {
  display: flex;
  align-items: center;
  margin: 20px 0;
}

.line {
  border-bottom: 1px solid #ccc;
  width: 50px;
}

.or-line span {
  margin: 0 10px;
}

@media (max-width: 1440px) {
  .section-four {
    flex-direction: column;
    align-items: flex-start;
  }
  
  .text {
    font-size: 36px;
    line-height: 44px;
  }
  
  .form-section {
    width: 100%;
    margin: 20px 0;
  }
}

@media (max-width: 1024px) {
  .text {
    font-size: 30px;
    line-height: 38px;
  }
  
  .form-section {
    width: 90%;
  }
}

@media (max-width: 768px) {
  .text {
    font-size: 26px;
    line-height: 34px;
  }
  
  .form-section {
    width: 100%;
  }
  
  input,
  button {
    width: 100%;
  }
}

@media (max-width: 480px) {
  .text {
    font-size: 22px;
    line-height: 30px;
  }
  
  .form-section {
    padding: 10px;
  }
  
  input,
  button {
    width: 100%;
    height: 45px;
  }
}
</style>
