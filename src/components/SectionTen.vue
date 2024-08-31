<template>
  <div class="section-ten">
    <div class="content-wrapper">
      <h1 class="p">Plans & Pricing</h1>
      <p class="start">
        Startup Framework is free forever - you only pay for custom domain
        hosting or to export your site.
      </p>
      <div class="plans-container">
        <div class="plan starter">
          <h2>Starter</h2>
          <p class="price">9.99</p>
          <p class="details">2GB of Space</p>
          <p class="details">14 days backups</p>
          <p class="details">Social integration</p>
          <p class="details">Client billing</p>
          <p class="details">Remote access</p>
          <p class="details">Custom domain</p>
          <p class="details">24 hours support</p>
          <p class="details">Admin tools</p>
          <p class="details">Collaboration</p>
          <p class="details">User management</p>
          <button class="get-started">Get Started</button>
        </div>
        <div class="plan professional">
          <h2>Professional</h2>
          <p class="price">19.99</p>
          <p class="details">2GB of Space</p>
          <p class="details">14 days backups</p>
          <p class="details">Social integration</p>
          <p class="details">Client billing</p>
          <p class="details">Remote access</p>
          <p class="details">Custom domain</p>
          <p class="details">24 hours support</p>
          <p class="details">Admin tools</p>
          <p class="details">Collaboration</p>
          <p class="details">User management</p>
          <button class="get-started red">Get Started</button>
        </div>
        <div class="plan team">
          <h2>Team</h2>
          <p class="price">49.99</p>
          <p class="details">2GB of Space</p>
          <p class="details">14 days backups</p>
          <p class="details">Social integration</p>
          <p class="details">Client billing</p>
          <p class="details">Remote access</p>
          <p class="details">Custom domain</p>
          <p class="details">24 hours support</p>
          <p class="details">Admin tools</p>
          <p class="details">Collaboration</p>
          <p class="details">User management</p>
          <button class="get-started">Get Started</button>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "SectionTen",
};
</script>

<style scoped>
.section-ten {
  text-align: center;
  background-image: url("/src/assets/Mask.png");
  background-size: cover;
  background-position: center;
  min-height: 100vh;
  position: relative;
  max-width: 100%;
  background-color: #2f1893;
}

.content-wrapper {
  max-width: 1200px;
  margin: 0 auto;
  padding: 20px;
  color: #fff;
}

.plans-container {
  display: flex;
  justify-content: space-around;
  gap: 20px;
  flex-wrap: wrap;
}

.plan {
  min-width: 250px;
  border: 1px solid grey;
  padding: 20px;
  box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
  display: block;
  color: #fff;
  margin-top: 5px;
}

.p {
  padding-top: 64.2px;
  padding-left: 69px;
  padding-right: 30px;
  margin-bottom: 56px;
  font-family: "DM Sans";
  font-size: 42px;
  letter-spacing: -0.4px;
  text-align: center;
}

.start {
  justify-content: center;
  line-height: 32px;
  font-family: "DM Sans";
  font-size: 22px;
  text-align: center;
  margin: 0 auto 20px;
  width: 586px;
}

.plan h2 {
  margin-left: 69px;
  color: #fff;
  font-weight: 500;
  font-family: "DM Sans";
  font-size: 22px;
  line-height: 32px;
  text-align: left;
}

.plan .price {
  font-size: 45px;
  margin: 0 0 10px;
  color: #fff;
}

.plan .details {
  display: block;
  color: #fff;
  font-weight: 500;
  text-align: left;
  margin-left: 44px;
  font-family: "DM Sans", sans-serif;
  font-size: 16px;
  line-height: 26px;
  width: 118px;
  height: 26px;
}

.get-started {
  padding: 17px 60px;
  border-radius: 100px;
  color: white;
  background-color: rgb(47, 80, 94);
  border-radius: 20px;
  cursor: pointer;
  margin-top: 30.6px;
  margin-bottom: 56px;
  border: none;
}

.get-started.red {
  background-color: #e93a7d;
}

/* Responsive Styles */
@media (max-width: 1440px) {
  .content-wrapper {
    padding: 15px;
  }
  .plan .details {
    margin-left: 35px;
  }
}

@media (max-width: 1200px) {
  .p {
    font-size: 36px;
  }
  .start {
    font-size: 20px;
    width: 500px;
  }
  .plans-container {
    gap: 15px;
  }
  .plan h2 {
    margin-left: 60px;
  }
  .plan .details {
    margin-left: 35px;
  }
}

@media (max-width: 1024px) {
  .p {
    font-size: 32px;
  }
  .start {
    font-size: 18px;
    width: 400px;
  }
  .plans-container {
    gap: 10px;
  }
  .plan h2 {
    margin-left: 50px;
  }
  .plan .details {
    margin-left: 30px;
  }
}

@media (max-width: 1000px) {
  .p {
    font-size: 30px;
  }
  .start {
    font-size: 17px;
    width: 380px;
  }
  .plans-container {
    gap: 10px;
  }
  .plan h2 {
    margin-left: 48px;
  }
  .plan .details {
    margin-left: 28px;
  }
}

@media (max-width: 900px) {
  .p {
    font-size: 28px;
  }
  .start {
    font-size: 16px;
    width: 350px;
  }
  .plans-container {
    flex-direction: column;
    align-items: center;
  }
  .plan {
    width: 90%;
    margin-bottom: 20px;
  }
}

@media (max-width: 810px) {
  .p {
    font-size: 26px;
  }
  .start {
    font-size: 15px;
    width: 330px;
  }
  .plan h2 {
    margin-left: 45px;
  }
  .plan .details {
    margin-left: 25px;
  }
  .get-started {
    padding: 15px 50px;
  }
}

@media (max-width: 768px) {
  .p {
    font-size: 24px;
  }
  .start {
    font-size: 14px;
    width: 320px;
    margin-left: 0;
  }
  .plan h2 {
    margin-left: 40px;
  }
  .plan .details {
    margin-left: 20px;
  }
}

@media (max-width: 480px) {
  .p {
    font-size: 22px;
    padding-left: 20px;
    padding-right: 20px;
  }
  .start {
    font-size: 12px;
    width: 280px;
  }
  .plan h2 {
    margin-left: 30px;
  }
  .plan .details {
    margin-left: 15px;
  }
  .get-started {
    padding: 12px 40px;
  }
}
</style>
