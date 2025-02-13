<template>
  <div class="testimonial-card">
    <div class="testimonial-content">
      <h4 class="testimonial-name">{{ name }}</h4>
      <p class="testimonial-text">{{ text }}</p>
      <div class="testimonial-quotes">❝❞</div>
      <div class="testimonial-rating">
        <span v-for="star in 5" :key="star" class="star">★</span>
      </div>
    </div>
    <div class="testimonial-image">
      <img :src="imageSrc" alt="Testimonial Image" class="image">
      <div class="play-button">
        <button @click="playVideo">
          <img :src="playIcon" alt="Play">
        </button>
      </div>
    </div>
  </div>
</template>

<script setup>
defineProps({
  name: String,
  text: String,
  imageSrc: String,
  playIcon: String
});

const playVideo = () => {
  alert('Reproducir video...');
};
</script>

<style scoped>
.testimonial-card {
  display: flex;
  align-items: center;
  background: white;
  padding: 20px;
  border-radius: 30px;
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
  max-width: 600px;
}

.testimonial-content {
  flex: 1;
  padding-right: 20px;
}

.testimonial-name {
  font-size: 1.5rem;
  font-weight: bold;
  margin-bottom: 5px;
}

.testimonial-text {
  font-size: 1rem;
  color: #333;
}

.testimonial-quotes {
  font-size: 2rem;
  color: #ddd;
  margin: 10px 0;
}

.testimonial-rating {
  color: gold;
  font-size: 1.2rem;
}

.testimonial-image {
  position: relative;
  width: 250px;
}

.image {
  width: 100%;
  border-radius: 10px;
}

.play-button {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
}

.play-button button {
  background: rgba(255, 215, 0, 0.8);
  border: none;
  padding: 10px;
  border-radius: 50%;
  cursor: pointer;
}

.play-button img {
  width: 30px;
}

@media (max-width: 768px) {
  .testimonial-card {
    flex-direction: column;
    text-align: center;
    max-width: 90%;
    padding: 15px;
  }

  .testimonial-content {
    padding-right: 0;
    margin-bottom: 15px;
  }

  .testimonial-name {
    font-size: 1.3rem;
  }

  .testimonial-text {
    font-size: 0.9rem;
  }

  .testimonial-quotes {
    font-size: 1.8rem;
  }

  .testimonial-rating {
    font-size: 1rem;
  }

  .testimonial-image {
    width: 200px;
  }

  .play-button img {
    width: 25px;
  }
}

@media (max-width: 480px) {
  .testimonial-card {
    max-width: 100%;
    padding: 10px;
  }

  .testimonial-name {
    font-size: 1.2rem;
  }

  .testimonial-text {
    font-size: 0.85rem;
  }

  .testimonial-quotes {
    font-size: 1.6rem;
  }

  .testimonial-rating {
    font-size: 0.9rem;
  }

  .testimonial-image {
    width: 180px;
  }

  .play-button img {
    width: 20px;
  }

  .play-button button {
    padding: 8px;
  }
}
</style>
