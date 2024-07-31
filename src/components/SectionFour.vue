<template>
  <div class="section-four">
    <div class="content">
      <div class="text">
        <h2>We solve digital problems with an outstanding creative flare</h2>
        <p>We have created a new product that will help designers, developers, and companies create websites for their startups quickly and easily.</p>
      </div>
      <div class="form">
        <form @submit.prevent="handleSubmit">
          <div class="form-group">
            <label placeholder="Your Email" for="email">Your email</label>
            <input type="email" id="email" v-model="email" required>
          </div>
          <div class="form-group">
            <label placeholder="Your Password" for="password">Your Password</label>
            <input type="password" id="password" v-model="password" required>
          </div>
          <button type="submit" class="btn-primary">Create an Account</button>
          <button type="button" class="btn-secondary">Login via Twitter</button>
        </form>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      email: '',
      password: ''
    };
  },
  methods: {
    handleSubmit() {
      // Handle form submission
      console.log('Form submitted', this.email, this.password);
    }
  }
};
</script>

<style scoped>
.section-four {
  display: flex;
  justify-content: center;
  align-items: center;
  background-image: url('/public/Image.png');
  background-size: cover;
  background-position: center;
  color: white;
  padding: 20px;
  min-height: 100vh;
  text-align: left;
}

.content {
  display: flex;
  flex-direction: column;
  max-width: 1200px;
  width: 100%;
  padding: 20px;
  border-radius: 10px;
}

.text {
  flex: 1;
}

.text h2 {
  margin-bottom: 10px;
  font-size: 23px;
  font-weight: 500;

}

.text p {
  margin-bottom: 20px;
  font-size: 12px;
}

.form {
  flex: 1;
  display: flex;
  flex-direction: column;
  justify-content: center;
  background-color: white;
  padding: 20px;
  border-radius: 10px;
  color: gray;
}

.form-group {
  margin-bottom: 15px;
}

.form-group label {
  display: block;
  margin-bottom: 5px;
}

.form-group input {
  width: 100%;
  padding: 10px;
  border-radius: 5px;
  border: 1px gray solid;
}

.btn-primary,
.btn-secondary {
  width: 100%;
  padding: 10px;
  border-radius: 5px;
  border: none;
  color: white;
  cursor: pointer;
  margin-bottom: 10px;
  background-color: #1DA1F2;
}

.btn-primary {
    background: #25DAC5;
}

.btn-secondary {
  background-color: #1DA1F2; 
}

@media (min-width: 768px) {
  .content {
    flex-direction: row;
  }

  .text, .form {
    flex: 1;
  }
}
</style>
