<template>
  <div class="section-four">
    <div class="text-section">
      <h1>We solve digital <br> problems with an <br> outstanding  <br>creative flare</h1>
      <p>We have created a new product that will help <br> designers, developers, and companies create <br> websites for their startups quickly and easily.</p>
    </div>
    <div class="form-section">
      <div class="sign-up-form" v-show="showSignUp">
        <h2>Sign Up</h2>
        <input type="email" placeholder="Your email" />
        <input type="password" placeholder="Your password" />
        <button>Create an Account</button>
        <button class="twitter-button">Login via Twitter</button>
        <div class="switch-form">
          <hr />
          <span @click="toggleForm">Already have an account? Login</span>
        </div>
      </div>
      <div class="login-form" v-show="!showSignUp">
        <h2>Login</h2>
        <input type="email" placeholder="Your email" />
        <input type="password" placeholder="Your password" />
        <button>Login</button>
        <button class="twitter-button">Login via Twitter</button>
        <div class="switch-form">
          <hr />
          <span @click="toggleForm">Don't have an account? Sign Up</span>
        </div>
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
    toggleForm() {
      this.showSignUp = !this.showSignUp;
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
  min-height: 100vh;
  position: relative;
  max-width: 100%;
  background-color: blue;
}

/* Text Section */
.text-section {
  width: 50%;
  padding: 20px;
}

.form-section {
  width: 400px;
  background: white;
  color: black;
  padding: 20px;
  border-radius: 10px;
  box-shadow: 10px rgba(0, 0, 0, 0.1);
  margin-right: 65px;
  padding-right: 40px;
}

/* Input Styles */
input {
  width: 100%;
  padding: 10px;
  margin: 10px 0;
  border: 1px solid #ccc;
  border-radius: 5px;
}

/* Button Styles */
button {
  width: 100%;
  padding: 10px;
  margin: 10px 0;
  border: none;
  border-radius: 5px;
  background: #25DAC5;
  color: white;
  cursor: pointer;
}

.twitter-button {
  background:#1DA1F2;
}

/* Switch Form */
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
