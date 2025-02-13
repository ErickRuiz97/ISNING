<template>
  <section class="contact-us-section">
    <div class="text-content">
      <h1>Ready to <br /> Get Started?</h1>
      <p>
        Whether you're planning a stunning outdoor retreat, or a major construction project, Vintage Outdoor Inc. and Vintage Construction Inc. are here to help.
      </p>
      <p>
        Get in touch with us today to discuss your project, request a quote, or schedule a consultation.
      </p>

      <div class="contact-info">
        <div class="contact-item">
          <i class="fa fa-phone icon-style"></i>
          <div class="phone-number">
            <small><strong>Phone Number</strong></small>
            <span>760 350 5552</span>
          </div>
        </div>
        <div class="contact-item">
          <i class="fa fa-map-marker icon-style"></i>
          <div class="address">
            <small><strong>Address</strong></small>
            <span>123 Main Street, Suite 456, Your city, ST 78901</span>
          </div>
        </div>
      </div>
    </div>

    <div class="contact-form-card">
      <h2>Send a Message</h2>
      <form @submit.prevent="submitForm">
        <input type="text" placeholder="Name" required />
        <input type="email" placeholder="E-mail address" required />
        <textarea placeholder="Message" required></textarea>
        <button type="submit" class="submit-btn">Submit</button>
      </form>
    </div>
  </section>
</template>

<script setup>
import { ref } from 'vue';

const submitForm = () => {
  console.log('Form submitted');
};
</script>

<style scoped>
.icon-style {
  display: inline-flex;
  justify-content: center;
  align-items: center;
  width: 30px;
  height: 30px;
  background-color: #C49326;
  color: white;
  border-radius: 50%;
  font-size: 1.5rem;
  padding: 5px;
}

.contact-us-section {
  display: flex;
  justify-content: space-between;
  padding: 50px;
  gap: 30px;
}

.text-content {
  flex: 1;
}

h1 {
  font-size: 2.5rem;
  font-weight: bold;
}

p {
  font-size: 1rem;
  margin: 15px 0;
}

.contact-info {
  margin-top: 20px;
}

.contact-item {
  display: flex;
  align-items: center;
  margin-bottom: 20px;
}

.contact-item i {
  font-size: 1.5rem;
  margin-right: 10px;
}

.contact-item small {
  font-size: 0.8rem;
  color: #555;
  display: block;
}

.contact-item span {
  font-size: 1.2rem;
  color: #333;
}

.contact-form-card {
  background-color: #fff;
  padding: 30px;
  border-radius: 20px;
  box-shadow: 0 4px 12px rgba(0, 0, 0, 0.1);
  width: 400px;
  flex: 1;
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  max-width: 550px;
  min-height: 550px;
}

.contact-form-card h2 {
  font-size: 3.0rem;
  margin-bottom: 20px;
  text-align: center;
}

.contact-form-card form {
  display: flex;
  flex-direction: column;
  flex-grow: 1;
  margin-top: 0;
}

.contact-form-card input,
.contact-form-card textarea {
  padding: 15px;
  margin-bottom: 20px;
  border: none;
  border-bottom: 2px solid #ddd;
  font-size: 1.2rem;
  width: 100%;
}

.contact-form-card input:focus,
.contact-form-card textarea:focus {
  outline: none;
  border-bottom: 2px solid #ddd;
}

.contact-form-card button.submit-btn {
  background-color: #C49326;
  color: white;
  padding: 15px 25px;
  border: none;
  border-radius: 10px;
  font-size: 1.3rem;
  cursor: pointer;
  align-self: flex-end;
  font-weight: bold;
}

.contact-form-card button.submit-btn:hover {
  background-color: #a17a21;
}
</style>
