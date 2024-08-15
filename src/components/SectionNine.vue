<template>
    <section class="section-nine">
      <div class="contact-info">
        <h1 class="Let">Let's Keep in Touch</h1>
        <p class="We">We have reated a new product that will help designers, developers, and companies create websites for their startups quickly and easily.</p>
        <div class="contact-details">
          <p class="date"><i class="fa fa-phone"></i> +233 257732425</p>
          <p class="date"><i class="fa fa-envelope"></i> patrickafriyiewilson12345@gmail.com</p>
          <p class="date"><i class="fa fa-map-marker"></i> Sekondi-Takoradi, Danielson Street</p>
        </div>
      </div>
      <div class="form-container">
        <form>
          <div class="form-group">
            <label for="name">Your Name</label>
            <input type="text" id="name" name="name" placeholder="First Name" required>
          </div>

          <div class="form-group">
            <label for="Input field">Input field</label>
            <input type="text" id="Input field" name="Input field" placeholder="patrick123@gmail.com" required>
          </div>

          <div class="form-group">
            <label for="budget">Budget</label>
            <input type="text" id="budget" name="budget" placeholder="$500" required>
          </div>

          <div class="form-group">
            <label for="message">Your Message</label>
            <textarea id="message" name="message" placeholder="Your Message" required></textarea>
          </div>
          <div class="form-group">
            <button type="submit" class="send-button">Send</button>
            <label>
              <input type="checkbox" name="send_copy">
              Send me a copy
            </label>
          </div>
        </form>
      </div>
    </section>
  </template>
  
  <script>
  export default {
    name: 'SectionNine'
  }
  </script>
  
  <style scoped>
  .section-nine {
    display: flex;
    justify-content: space-between;
    align-items: flex-start;
    padding-left: 150px;
    padding-right: 150px;
    padding-top: 70px;
    background-image: url('/src/assets/Background%20(3).png');
    color: white;
    min-height: 100vh;
    position: relative;
    max-width: 100%;
    background-color: #2F1893;
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
letter-spacing: -0.4000000059604645px;
text-align: left;


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

  }

  .date {
    margin-top: 40px;
    font-size: 15px;
    font-weight: 500;
    width: 283.5px;
  }
  
  .contact-details i {    margin-right: 10px;
  }
  
  .form-container {
    width: 35%;
    background-color: white;
    color: black;
    padding: 40px;
    border-radius: 10px;
    margin-right: 60px;
  }
  
  .form-group {
    display: flex;
    flex-direction: column;
    margin-bottom: 15px;
    max-width: 470px;
max-height: 570px;
}
  
  .form-group label {
    margin-bottom: 5px;
  }
  
  .form-group input,
  .form-group textarea {
    padding: 10px;
    border: 1px solid #ccc;
    border-radius: 13px;
  }
  
  .send-button {
    background-color: blue;
    color: white;
    padding: 10px 20px;
    border: none;
    border-radius: 3px;
    cursor: pointer;
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
  }
  </style>
  