<template>
  <div class="contact-us-container">
    <div class="overlay"></div>
    <img src="https://st.depositphotos.com/68974274/60910/i/450/depositphotos_609101630-stock-photo-wonderful-waves-surface-pool-steps.jpg" alt="Contact Us" class="contact-us-image" />
    <div class="contact-us-text">Contact Us</div>
  </div>
</template>

<style scoped>
.contact-us-container {
  position: relative;
  display: flex;
  justify-content: center;
  align-items: flex-start;
  width: 100%;
}

.contact-us-image {
  width: 100%;
  height: 350px;
  border-radius: 20px;
}

.overlay {
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  background-color: rgba(0, 0, 0, 0.5);
  border-radius: 20px;
}

.contact-us-text {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  color: white;
  font-size: 4rem;
  font-weight: bold;
  text-shadow: 2px 2px 5px rgba(0, 0, 0, 0.7);
}
</style>
