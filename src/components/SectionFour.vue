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
  align-items: center;
  background-image: url("/public/Image.png");
  background-size: cover;
  color: white;
  flex-wrap: wrap;
  height: 750px;
  max-width: 100%;
  background-color: #2f1893;
  font-family: "DM Sans", sans-serif;
}

.text {
  font-size: 42px;
  line-height: 52px;
  letter-spacing: -0.4px;
  text-align: left;
  margin-bottom: 32px;
  width: 368px;
  height: 208px;
  top: 216px;
  left: 216px;
  gap: 0px;
  opacity: 0px;
  margin-left: 216px;
  margin-right: 31px; 
}

.we {
  font-size: 16px;
  line-height: 26px;
  text-align: left;
  width: 369px;
  height: 78px;
  top: 456px;
  left: 216px;
  gap: 0px;
  opacity: 0px;
  margin-left: 216px;
  margin-right: 31px;

}

.form-section {
  width: 470px;
  height: 550px;
  background: white;
  color: black;
  border-radius: 10px;
  margin-right: 215px;
  margin-bottom: 100px;
  margin-top: 100px;
  margin-left: 31px;
}

.tab-container {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-bottom: 69px;
  padding-top: 25px;
}

.tablinks {
  flex: 1;
  padding: 10px;
  cursor: pointer;
  text-align: center;
  background-color: #fff;
  outline: none;
  color: gray;
  border: none;
}

.tablinks.active {
  border-bottom: 2px solid #1E0E62;
  background-color: white;
  font-weight: bold;
  border-radius: 0px;
}

input {
  width: 300px;
  height: 50px;
  border-radius: 100px;
  border: 2px solid #ccc;
  padding-left: 24px;
  display: block;
  margin-bottom: 30px;
  margin-right: 69px;
  margin-left: 71px;
}

button {
  width: 330px;
  height: 50px;
  border-radius: 100px;
  border: none;
  background: #25dac5;
  color: white;
  cursor: pointer;
  display: block;
  margin-left: 71px;
  padding-top: 12px;
  padding-bottom: 12px;
  margin-bottom: 19px;
  padding-left: 85px;
  padding-right: 85px;
}

.twitter-button {
  background: #1da1f2;
}

.or-line {
  display: flex;
  align-items: center;
  margin: 20px 0;
  justify-content: center;
}

.line {
  border-bottom: 1px solid #ccc;
  width: 50px;
}

.or-line span {
  margin: 0 18px;
  color:#141414
}

@media (max-width: 768px) {
  .section-four {
    flex-direction: column;
    align-items: flex-start;
  }

  .text {
    text-align: center;
    margin-left: 0;
  }

  .form-section {
    margin: 0 auto;
    width: 90%;
  }
}

@media (max-width: 480px) {
  .text {
    font-size: 24px;
    line-height: 34px;
  }

  .we {
    font-size: 12px;
    line-height: 18px;
  }

  .form-section {
    width: 100%;
    height: auto;
    padding: 20px;
  }

  input,
  button {
    width: 100%;
  }
}
</style>

