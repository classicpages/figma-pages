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
            <input type="text" id="name" name="name" required>
          </div>
          <div class="form-group">
            <label for="budget">Budget</label>
            <input type="text" id="budget" name="budget" required>
          </div>
          <div class="form-group">
            <label for="message">Your Message</label>
            <textarea id="message" name="message" required></textarea>
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
    padding: 20px;
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
    font-size: 30px;
    font-weight: 800;
  }

  .We {
    font-size: 16px;
    font-weight: 500;
    width: 300px;
    margin-top: 30px;
  }

  .date {
    margin-top: 40px;
    font-size: 15px;
    font-weight: 500;
  }
  
  .contact-details i {
    margin-right: 10px;
  }
  
  .form-container {
    width: 35%;
    background-color: white;
    color: black;
    padding: 20px;
    border-radius: 10px;
    margin-right: 60px;
  }
  
  .form-group {
    display: flex;
    flex-direction: column;
    margin-bottom: 15px;
  }
  
  .form-group label {
    margin-bottom: 5px;
  }
  
  .form-group input,
  .form-group textarea {
    padding: 10px;
    border: 1px solid #ccc;
    border-radius: 3px;
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
  