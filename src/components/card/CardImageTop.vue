<template>
  <div class="custom-card">
    <img :src="imageSrc" alt="Card Image" class="card-img">
    <div class="card-content">
      <h5 class="card-title">{{ title }}</h5>
      <p class="card-text">{{ subtitle }}</p>
      <button class="btn btn-light shadow-sm">Read More</button>
    </div>
  </div>
</template>

<script setup>
defineProps({
  imageSrc: String,
  title: String,
  subtitle: String
});
</script>

<style scoped>
.custom-card {
  position: relative;
  width: 320px;
  border-radius: 30px;
  height: auto;
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
}

.card-img {
  width: 100%;
  height: auto;
  display: block;
  border-radius: 30px;
}

.card-content {
  position: absolute;
  bottom: -50px;
  left: 50%;
  width: 85%;
  background: white;
  padding: 15px;
  border-radius: 12px;
  text-align: center;
  transform: translateX(-50%);
  box-shadow: 0 4px 10px rgba(0, 0, 0, 0.15);
  transition: 0.3s ease-in-out;
}

.card-title {
  font-size: 1rem;
  font-weight: bold;
  margin-bottom: 5px;
}

.card-text {
  font-size: 0.9rem;
  color: gray;
  margin-bottom: 10px;
}

@media (max-width: 400px) {
  .custom-card {
    width: 100%;
  }

  .card-content {
    width: 90%;
    bottom: -40px;
    padding: 10px;
  }

  .card-title {
    font-size: 0.9rem;
  }

  .card-text {
    font-size: 0.8rem;
  }

  .btn {
    font-size: 0.8rem;
    padding: 5px 10px;
  }
}
</style>
