<template>
  <footer class="footer">
    <div class="footer-top">
      <div class="footer-left">
        <p>Startup 3</p>
      </div>
      <div class="footer-right">
        <p>PrivacyPolicy Terms</p>
        <div class="icons">
          <i class="fab fa-twitter"></i>
          <i class="fab fa-facebook"></i>
          <i class="fab fa-google"></i>
        </div>
      </div>
    </div>
    <hr />
    <div class="footer-bottom">
      <div class="footer-links">
        <p>Tour</p>
        <p>Features</p>
        <p>Pricing</p>
        <p>Plans</p>
        <p>Our Works</p>
        <p>Brands</p>
        <p>Contacts</p>
      </div>
      <div class="footer-right">
        <p>2017 Designmodo. All rights reserved.</p>
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  name: "SectionEleven",
};
</script>

<style scoped>
.footer {
  background-color: #2f1893;
  color: white;
  padding: 20px;
  font-family: 'DM Sans' sans-serif;
  font-size: 16px;
  line-height: 26px;
  text-align: left;
}

.footer-top,
.footer-bottom {
  display: flex;
  justify-content: space-between;
  align-items: center;
  font-weight: 600;
  margin-left: 115px;
  margin-right: 115px;
  margin-bottom: 44px;
  margin-top: 47px;
  font-family: 'DM Sans' sans-serif;

}

.footer-left,
.footer-right {
  display: flex;
  align-items: center;
  font-weight: 500;
  font-family: 'DM Sans' sans-serif;
}

.footer-right .icons i {
  margin-left: 10px;
}

hr {
  border: 1px solid gray;
  margin: 20px 0;
}

.footer-links {
  display: flex;
  gap: 20px;
}

@media (max-width: 768px) {
  .footer-top,
  .footer-bottom {
    flex-direction: column;
    align-items: flex-start;
  }

  .footer-links {
    flex-wrap: wrap;
    gap: 10px;
  }
}
</style>
