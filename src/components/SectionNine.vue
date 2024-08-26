<template>
  <section class="section-nine">
    <div class="contact-info">
      <h1 class="Let">Let's Keep in Touch</h1>
      <p class="We">
        We have created a new product that will help designers, developers, and
        companies create websites for their startups quickly and easily.
      </p>
      <div class="contact-details">
        <p class="date"><i class="fa fa-phone"></i> +233 257732425</p>
        <p class="date">
          <i class="fa fa-envelope"></i> patrickafriyiewilson12345@gmail.com
        </p>
        <p class="date">
          <i class="fa fa-map-marker"></i> Sekondi-Takoradi, Danielson Street
        </p>
      </div>
    </div>
    <div class="form-container">
      <form>
        <div class="form-group">
          <label for="name">Your Name</label>
          <input
            type="text"
            id="name"
            name="name"
            placeholder="First Name"
            required
          />
        </div>

        <div class="form-group">
          <label for="email">Input field</label>
          <input
            type="email"
            id="email"
            name="email"
            placeholder="patrick123@gmail.com"
            required
          />
        </div>

        <div class="form-group">
          <label for="budget">Budget</label>
          <input
            type="text"
            id="budget"
            name="budget"
            placeholder="$500"
            required
          />
        </div>

        <div class="form-group">
          <label for="message">Your Message</label>
          <textarea
            id="message"
            name="message"
            placeholder="Your Message"
            required
          ></textarea>
        </div>

        <div class="form-group form-actions">
          <button type="submit" class="send-button">Send</button>

       
        </div>
       
      </form>
    </div>
  </section>
</template>

<script>
export default {
  name: "SectionNine",
};
</script>

<style scoped>
.section-nine {
  display: flex;
  justify-content: space-between;
  align-items: flex-start;
  background-image: url("/src/assets/Background%20(3).png");
  color: white;
  min-height: 100vh;
  position: relative;
  max-width: 100%;
  background-color: #2f1893;
}

.contact-info {
  width: 50%;
}

.Let {
  margin-top: 70px;
  font-weight: 800;
  width: 410px;
  height: 52px;
  font-size: 42px;
  line-height: 52px;
  letter-spacing: -0.4px;
  text-align: left;
  margin-top: 150px;
  margin-left: 215px;
}

.We {
  font-weight: 300;
  margin-top: 30px;
  width: 399px;
  height: 128px;
  top: 230px;
  left: 216px;
  font-size: 22px;
  line-height: 32px;
  text-align: left;
  margin-left: 215px;

}



.date {
  margin-top: 40px;
  font-size: 15px;
  font-weight: 500;
  width: 283.5px;
  margin-left: 215px;

}

.contact-details i {
  margin-right: 10px;
  margin-top: 53.2px;
}

.form-container {
  width: 470px;
  background-color: white;
  color: black;
  padding-left: 50px;
  padding-right: 50px;
  padding-top: 55px;
  border-radius: 10px;
  margin-bottom: 100px;
  margin-top: 100px;
  margin-right: 100px;
}

.form-group {
  display: flex;
  flex-direction: column;
  margin-bottom: 25px;
  max-width: 470px;
  max-height: 570px;
}

.form-group label {
  margin-bottom: 5px;
}


.form-group textarea {
  padding-left: 19px;
  padding-top: 12px;
  padding-bottom: 100px;
  border: 1px solid #ccc;
  border-radius: 13px;
}

.form-group input{
  border: 1px solid #ccc;
  border-radius: 100px;
  padding-left: 24px;
  padding-right: 84px;
  padding-top: 12px;
  padding-bottom: 12px;
}

.form-actions {
  display: flex;
  align-items:end;
}

.form-actions label {
  margin-bottom: 0;
}

.send-button {
  background-color: #25dac5;
  color: white;
  padding: 12px 36px;
  border: none;
  border-radius: 100px;
  cursor: pointer;
  width: 120px;
  height: 50px;
  margin-bottom: 56px;
}

.form-actions input[type="checkbox"]:checked {
  background-color: #25dac5;
  border-color: #25dac5;
}

@media (max-width: 768px) {
  .section-nine {
    flex-direction: column;
    align-items: center;
  }

  .contact-info,
  .form-container {
    width: 100%;
  }

  .form-actions {
    flex-direction: column;
    align-items: flex-start;
  }

  .send-button {
    width: 100%;
    margin-top: 15px;
  }
}

@media (max-width: 480px) {
  .section-nine {
    padding-left: 20px;
    padding-right: 20px;
  }

  .Let {
    font-size: 32px;
  }

  .We {
    font-size: 18px;
  }

  .form-actions {
    flex-direction: column;
    align-items: flex-start;
  }

  .send-button {
    width: 100%;
    margin-top: 15px;
  }
}
</style>
