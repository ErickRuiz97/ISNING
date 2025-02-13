<template>
  <div class="image-container">
    <img :src="imageUrl" alt="Card Image" class="oval-img">
    <div class="overlay-text">
      <h1 class="title">TRANSFORMING SPACES, BUILDING DREAMS</h1>
      <p class="subtitle">Landscaping | Outdoor Living | Construction Services</p>
      <div class="buttons">
        <button class="btn primary-btn">Explore Our Services</button>
        <button class="btn secondary-btn">View Our Work</button>
      </div>
    </div>
    <div class="vision-text">
      <p>From Vision to Reality, <br>Inside and Out</p>
    </div>
  </div>
</template>

<script setup>
const imageUrl = 'https://images.unsplash.com/photo-1600596542815-ffad4c1539a9?fm=jpg&q=60&w=3000&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxzZWFyY2h8Mnx8Y2FzYSUyMGRlJTIwbGElMjBwaXNjaW5hfGVufDB8fDB8fHww';
</script>

<style scoped>
.image-container {
  position: relative;
  display: flex;
  justify-content: center;
  align-items: flex-start;
  width: 100%;
}

.oval-img {
  width: 90vw;
  max-width: 1200px;
  height: 400px;
  object-fit: cover;
  border-radius: 15px;
}

.overlay-text {
  position: absolute;
  top: 15%;
  left: 5%;
  text-align: left;
}

.title {
  font-size: 2rem;
  font-weight: bold;
  color: #333333;
}

.subtitle {
  font-size: 1rem;
  margin-top: 5px;
  color: #333333;
}

.buttons {
  margin-top: 15px;
  display: flex;
  gap: 10px;
}

.btn {
  padding: 10px 20px;
  font-size: 1rem;
  font-weight: bold;
  border: none;
  cursor: pointer;
  border-radius: 15px;
  transition: background-color 0.3s, color 0.3s;
}

.primary-btn {
  background-color: #C49326;
  color: white;
}

.primary-btn:hover {
  background-color: #a5781e;
  color: white;
}

.secondary-btn {
  background-color: white;
  color: #C49326;
  border: 2px solid #C49326;
}

.secondary-btn:hover {
  background-color: white;
  color: #C49326;
  border-color: #C49326;
}

.vision-text {
  position: absolute;
  bottom: 0;
  right: 0;
  background-color: white;
  padding: 15px;
  border-top-left-radius: 25px;
  width: 250px;
  text-align: center;
  font-size: 1.2rem;
  font-weight: bold;
  color: #333333;
}

.vision-text p {
  margin: 0;
}

@media (max-width: 768px) {
  .overlay-text {
    top: 10%;
    left: 5%;
    width: 90%;
    text-align: center;
  }

  .title {
    font-size: 1.5rem;
  }

  .subtitle {
    font-size: 0.9rem;
  }

  .buttons {
    flex-direction: column;
    align-items: center;
  }

  .btn {
    width: 100%;
    font-size: 0.9rem;
    padding: 8px 15px;
  }

  .vision-text {
    width: 100%;
    position: static;
    border-radius: 0;
    padding: 10px;
    font-size: 1rem;
  }
}

@media (max-width: 480px) {
  .title {
    font-size: 1.2rem;
  }

  .subtitle {
    font-size: 0.8rem;
  }

  .btn {
    font-size: 0.8rem;
  }

  .oval-img {
    height: 250px;
  }
}
</style>
