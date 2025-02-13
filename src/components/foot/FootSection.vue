<template>
  <section class="footer-container">
    <div class="content-container">
      <div class="left-section">
        <div class="logo">
          <img
            src="https://le-cdn.hibuwebsites.com/be04dc16d67f484bbb4edb2b6e8fdff9/dms3rep/multi/opt/vintage-outdoor-inc-logo-300w.png"
            alt="Vintage Outdoor Logo" />
        </div>
        <p>
          At Vintage Outdoor Inc., we are passionate about transforming your outdoor spaces into breathing landscapes
          that enhance your lifestyle.
        </p>
        <div class="social-icons">
          <i class="fa fa-facebook icon-style"></i>
          <i class="fa fa-whatsapp icon-style"></i>
          <i class="fa fa-linkedin icon-style"></i>
          <i class="fa fa-twitter icon-style"></i>
        </div>
      </div>

      <div class="links-container">
        <div class="links-section">
          <div class="company-info">
            <strong>Our Company</strong>
            <ul>
              <li>Home</li>
              <li>About Us</li>
              <li>Services</li>
              <li>Vintage Construction</li>
              <li>Gallery</li>
            </ul>
          </div>
          <div class="support-info">
            <strong>Support</strong>
            <ul>
              <li>Testimonials</li>
              <li>Blogs</li>
              <li>FAQs</li>
              <li>Contact Us</li>
            </ul>
          </div>
        </div>
      </div>

      <div class="newsletter-contact">
        <div class="newsletter">
          <strong>Join Our Newsletter</strong>
          <div class="newsletter-input">
            <input type="email" placeholder="Enter your email" />
            <button class="subscribe-btn">Subscribe</button>
          </div>
        </div>

        <div class="contact-info">
          <div class="contact-item">
            <i class="fa fa-phone icon-style"></i>
            <span>760 350 5552</span>
          </div>
          <div class="contact-item">
            <i class="fa fa-map-marker icon-style"></i>
            <span>123 Main Street, Suite 456, Your city, ST 78901</span>
          </div>
          <div class="contact-item">
            <i class="fa fa-envelope icon-style"></i>
            <span>office@vintageoutdoorinc.com</span>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
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

.footer-container {
  background: url("https://wallpapers.com/images/hd/pool-background-0xivea9tpv8t4gyv.jpg") no-repeat center center / cover;
  display: flex;
  justify-content: center;
  align-items: flex-start;
  width: 100%;
  margin: 0;
  border-radius: 20px;
}

.content-container {
  width: 100%;
  display: flex;
  justify-content: space-between;
  gap: 30px;
  background-color: rgba(255, 255, 255, 0.5);
  padding: 100px;
  border-radius: 20px;
}

.left-section {
  flex: 1;
  display: flex;
  flex-direction: column;
  align-items: flex-start;
}

.left-section .logo img {
  width: 120px;
  margin-bottom: 20px;
}

.left-section p {
  font-size: 1.2rem;
  margin-bottom: 15px;
}

.social-icons {
  display: flex;
  gap: 15px;
  font-size: 1.5rem;
}

.social-icons i {
  cursor: pointer;
}

.links-container {
  flex: 1;
}

.links-section {
  display: flex;
  justify-content: space-between;
  gap: 20px;
}

.company-info,
.support-info {
  flex: 1;
}

.company-info strong,
.support-info strong,
.newsletter strong {
  font-size: 1.2rem;
  font-weight: bold;
  display: block;
  margin-bottom: 10px;
}

.company-info ul,
.support-info ul {
  list-style: none;
  padding-left: 0;
}

.company-info li,
.support-info li {
  font-size: 1rem;
  margin: 5px 0;
  cursor: pointer;
}

.newsletter-contact {
  flex: 1;
  display: flex;
  flex-direction: column;
}

.newsletter {
  margin-bottom: 20px;
}

.newsletter-input {
  position: relative;
  display: flex;
  align-items: center;
  width: 100%;
}

.newsletter-input input {
  padding: 10px 20px;
  border-radius: 25px;
  border: 1px solid #ddd;
  font-size: 1rem;
  width: 100%;
  padding-right: 120px;
  /* Espacio para el botón */
}

.newsletter-input button.subscribe-btn {
  position: absolute;
  right: 5px;
  top: 50%;
  transform: translateY(-50%);
  background-color: #c49326;
  color: white;
  padding: 10px 15px;
  border: none;
  border-radius: 20px;
  font-size: 1rem;
  cursor: pointer;
}

.newsletter-input button.subscribe-btn:hover {
  background-color: #a17a21;
}


.contact-info {
  display: flex;
  flex-direction: column;
  justify-content: center;
}

.contact-item {
  display: flex;
  align-items: center;
  margin-bottom: 15px;
}

.contact-item i {
  font-size: 1.5rem;
  margin-right: 10px;
}

.contact-item span {
  font-size: 1rem;
}

@media (max-width: 1024px) {
  .content-container {
    flex-direction: column;
    align-items: center;
    padding: 50px;
    text-align: center;
  }

  .left-section,
  .links-container,
  .newsletter-contact {
    width: 100%;
    align-items: center;
    text-align: center;
  }

  .links-section {
    flex-direction: column;
    gap: 15px;
    align-items: center;
  }

  .company-info ul,
  .support-info ul {
    padding-left: 0;
  }

  .social-icons {
    justify-content: center;
  }
}

@media (max-width: 768px) {
  .content-container {
    padding: 30px;
  }

  .newsletter-input {
    flex-direction: column;
  }

  .newsletter-input input {
    width: 100%;
    margin-bottom: 10px;
    padding-right: 20px;
  }

  .newsletter-input button.subscribe-btn {
    position: static;
    width: 100%;
    transform: none;
  }
}

@media (max-width: 480px) {
  .footer-container {
    border-radius: 0;
  }

  .content-container {
    padding: 20px;
  }

  .icon-style {
    width: 25px;
    height: 25px;
    font-size: 1.2rem;
  }

  .left-section p {
    font-size: 1rem;
  }

  .company-info strong,
  .support-info strong,
  .newsletter strong {
    font-size: 1rem;
  }

  .contact-item span {
    font-size: 0.9rem;
  }
}
</style>
