<template>
  <div class="section-four">
    <div class="text-section">
      <h1>We solve digital problems with an outstanding creative flare</h1>
      <p>We have created a new product that will help designers, developers, and companies create websites for their startups quickly and easily.</p>
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
  background: url('/public/Image.png') no-repeat center center;
  background-size: cover;
  color: white;
  padding: 20px;
  height: 100vh;
}

.text-section {
  width: 50%;
  padding: 20px;
}

.form-section {
  width: 40%;
  background: white;
  color: black;
  padding: 20px;
  border-radius: 10px;
  box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
}

input {
  width: 100%;
  padding: 10px;
  margin: 10px 0;
  border: 1px solid #ccc;
  border-radius: 5px;
}

button {
  width: 100%;
  padding: 10px;
  margin: 10px 0;
  border: none;
  border-radius: 5px;
  background: blue;
  color: white;
  cursor: pointer;
}

.twitter-button {
  background: #1da1f2;
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
</style>
