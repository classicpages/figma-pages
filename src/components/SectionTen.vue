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
          <p class="details">Collaboration tools</p>
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
          <p class="details">Collaboration tools</p>
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
          <p class="details">Collaboration tools</p>
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
  padding: 20px;
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
  text-align: center;
  font-family: "DM Sans";
  font-size: 42px;
  letter-spacing: -0.4000000059604645px;
  text-align: center;
}

.start {
  height: 64px;
  justify-content: center;
  line-height: 32px;
  text-align: center;
  width: 586px;
  height: 64px;
  font-family: "DM Sans";
  font-size: 22px;
  line-height: 32px;
  text-align: center;
  margin-left: 350px;
  margin-bottom: 20px;
}

.plan h2 {
  margin: 0 0 10px;
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
  margin-bottom: 10px;
  color: #fff;
  font-size: 15px;
  font-weight: 500;
}

.get-started {
  padding: 10px 20px;
  border: none;
  color: white;
  background-color: rgb(47, 80, 94);
  border-radius: 20px;
  cursor: pointer;
  margin-top: 30px;
}

.get-started.red {
  background-color: #e93a7d;
}

@media (max-width: 768px) {
  .plans-container {
    flex-direction: column;
    align-items: center;
  }
}
</style>
