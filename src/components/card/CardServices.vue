<template>
  <div class="custom-card">
    <img :src="imageSrc" alt="Card Image" class="card-img">
    <div class="card-body">
      <h5 class="card-title">{{ title }}</h5>
      <div class="card-text-container">
        <p v-if="details" class="card-text">{{ details }}</p>
      </div>
      <button class="btn shadow-button">
        Read More
        <span class="icon">
          <i class="fa fa-arrow-right icon-style"></i>
        </span>
      </button>
    </div>
  </div>
</template>

<script setup>
defineProps({
  imageSrc: String,
  title: String,
  details: String,
  iconSrc: String
});
</script>

<style scoped>
.icon-style {
  display: inline-flex;
  justify-content: center;
  align-items: center;
  width: 20px;
  height: 20px;
  background-color: #C49326;
  color: white;
  border-radius: 50%;
  font-size: 0.8rem;
  padding: 5px;
}
.custom-card {
  width: 350px;
  border-radius: 15px;
  overflow: hidden;
  background: white;
  padding-bottom: 20px;
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
}

.card-img {
  width: 100%;
  height: 200px;
  object-fit: cover;
}

.card-body {
  padding: 20px;
  text-align: center;
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  height: 300px;
}

.card-title {
  font-size: 1.5rem;
  font-weight: bold;
  color: #B8860B;
  margin-bottom: 15px;
}

.card-text-container {
  flex-grow: 1;
  display: flex;
  align-items: flex-start;
  justify-content: flex-start;
}

.card-text {
  font-size: 0.9rem;
  color: #333;
  text-align: left;
  padding-left: 10px;
}

.btn {
  display: flex;
  align-items: center;
  justify-content: center;
  width: 90%;
  margin: auto;
  border-radius: 25px;
  font-weight: bold;
  background-color: #f8f9fa;
  padding: 10px 20px;
  border: none;
}

.shadow-button {
  box-shadow: 0px 8px 16px rgba(0, 0, 0, 0.2);
}

.icon {
  margin-left: 10px;
  display: flex;
  align-items: center;
}

.icon img {
  width: 20px;
  height: 20px;
}

@media (max-width: 768px) {
  .custom-card {
    width: 90%;
    max-width: 350px;
    padding-bottom: 15px;
  }

  .card-img {
    height: 180px;
  }

  .card-body {
    padding: 15px;
    height: auto;
  }

  .card-title {
    font-size: 1.3rem;
    margin-bottom: 10px;
  }

  .card-text {
    font-size: 0.85rem;
    padding-left: 5px;
  }

  .btn {
    width: 100%;
    font-size: 0.9rem;
    padding: 8px 15px;
  }
}

@media (max-width: 480px) {
  .custom-card {
    width: 100%;
    padding-bottom: 10px;
  }

  .card-img {
    height: 150px;
  }

  .card-title {
    font-size: 1.2rem;
  }

  .card-text {
    font-size: 0.8rem;
  }

  .btn {
    font-size: 0.8rem;
  }

  .icon img {
    width: 16px;
    height: 16px;
  }
}
</style>
