<template>
  <div class="section-four">
    <div class="text-section">
      <h1 class="text">We solve digital <br> problems with an <br> outstanding  <br>creative flare</h1>
      <p class="we">We have created a new product that will help <br> designers, developers, and companies create <br> websites for their startups quickly and easily.</p>
    </div>
    <div class="form-section">
      <div class="tab-container">
        <button :class="['tablinks', { active: showSignUp }]" @click="toggleForm(true)">Sign Up</button>
        <button :class="['tablinks', { active: !showSignUp }]" @click="toggleForm(false)">Login</button>
      </div>
      
      <div class="sign-up-form" v-show="showSignUp">
        <h2></h2>
        <input type="email" placeholder="Your email" />
        <input type="password" placeholder="Your password" />
        <button>Create an Account</button>
        <button class="twitter-button">Login via Twitter</button>
      </div>
      <div class="login-form" v-show="!showSignUp">
        <h2></h2>
        <input type="email" placeholder="Your email" />
        <input type="password" placeholder="Your password" />
        <button>Login</button>
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
.section-four {
  display: flex;
  justify-content: space-between;
  align-items: center;
  background-image: url('/public/Image.png');
  background-size: cover;
  color: white;
  padding: 20px;
  flex-wrap: wrap;
  max-width: 1400px;
    height: 750px;
  position: relative;
  max-width: 1400px;
  background-color: #2F1893;
}

/* Text Section */
.text-section {
  width: 40%;
  padding: 20px;
  margin-left: 120px;
}

.we {
  font-size: 16px;
  line-height: 20px;
}

.form-section {
  width: 330px; 
  background: white;
  color: black;
  padding-left: 30px;
  padding-right: 30px;
  padding-top: 0;
  padding-bottom: 30px;
  border-radius: 15px;
  box-shadow: 5px rgba(0, 0, 0, 0.1);
  margin-right: 140px;
}

.tab-container {
  display: flex;
  justify-content: space-around;
  margin-bottom: 20px;
  border-bottom: 2px solid #ddd;
}

.tablinks {
  flex: 1;
  padding: 14px 16px;
  cursor: pointer;
  text-align: center;
  background-color: #f1f1f1;
  border: none;
  outline: none;
  color: #000;
  transition: background-color 0.3s;
}

.tablinks.active {
  border-bottom: 4px solid blue;
  font-weight: bold;
  background-color: white;
}

input {
  width: 73%;
  padding: 10px;
  margin: 10px 0;
  border: 1px solid #ccc;
  border-radius: 35px;
}

button {
  width: 80%;
  padding: 10px;
  margin: 10px 0;
  border: none;
  border-radius: 20px;
  background: #25DAC5;
  color: white;
  cursor: pointer;
}

.twitter-button {
  background:#1DA1F2;
}

.switch-form {
  text-align: center;
  margin-top: 10px;
}

.switch-form span {
  color: blue;
  cursor: pointer;
}

.switch-form hr {
  margin: 10px 0;
}

/* Responsive Styles */
@media (max-width: 1024px) {
  .text-section {
    width: 45%;
  }
  
  .form-section {
    width: 50%;
  }
}

@media (max-width: 768px) {
  .text-section {
    width: 100%;
    text-align: center;
    padding: 10px;
  }

  .form-section {
    width: 100%;
    margin-top: 20px;
    padding: 15px;
  }
}

@media (max-width: 480px) {
  .text-section {
    padding: 5px;
  }

  .form-section {
    padding: 10px;
  }

  input,
  button {
    padding: 8px;
  }
}

</style>
