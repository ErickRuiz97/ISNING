<template>
  <div class="container mt-5">
    <div class="row align-items-start">
      <div class="col-md-4">
        <img src="https://i.pinimg.com/736x/ff/4a/2d/ff4a2da2075c307ed46915bb194beaca.jpg"
          class="img-fluid mb-3 rounded-img" />
        <img src="https://www.terrasmalt.com/wp-content/uploads/2020/06/coronacion-terracotta-piscina.jpg"
          class="img-fluid rounded-img" />
      </div>
      <div class="col-md-8 ps-4">
        <h1 class="display-5 title-with-divider">Welcome to Vintage Outdoor Inc.</h1>
        <div class="pencil-divider p-0 mt-0"></div>
        <p class="custom-text first-paragraph">
          At Vintage Outdoor Inc., we are passionate about transforming your outdoor
          <br /> spaces into breathing landscapes that enhance your lifestyle.
        </p>
        <div class="card mb-4" style="background-color: #F9F9FB; border: none; border-radius: 20px;">
          <div class="card-body">
            <p class="custom-text mb-0">
              With years of expertise in custom design, installation, and
              maintenance, our goal is to bring your vision to life, whether
              you're dreaming of a serene garden, a luxurious outdoor living
              space, or a vibrant and functional yard.
            </p>
          </div>
        </div>
        <div class="card" style="background-color: #F9F9FB; border: none; border-radius: 20px;">
          <div class="card-body">
            <p class="custom-text mb-1">
              But we don't just stop at the outdoors. We're excited to introduce
              Vintage Construction Inc., a new division of our company
              specializing in high-quality construction services. From new home
              builds to remodels, ADUs, and commercial projects, Vintage
              Construction Inc. is here to make your construction dreams a
              reality.
            </p>
          </div>
        </div>
        <button class="btn mt-2" style="background-color: #C49326; color: white;">
          Read More
        </button>
      </div>
    </div>
  </div>
</template>

<script setup>
</script>

<style scoped>
.display-5 {
  font-weight: 400;
  position: relative;
  display: inline-block;
}

.title-with-divider {
  text-align: center;
  margin-bottom: 20px;
}

.pencil-divider {
  width: 200px;
  height: 3px;
  background: linear-gradient(to right, transparent, #C49326 25%, #C49326 50%, #C49326 75%, transparent);
  margin: 10px auto;
  border-radius: 5px;
}

.custom-text {
  font-size: 1.2rem;
  font-weight: normal;
  color: #333333;
  line-height: 1.6;
}

.first-paragraph {
  font-size: 1.1rem;
  text-align: center;
}

img {
  width: 100%;
  margin-bottom: 15px;
  border-radius: 30px;
}

.col-md-4 {
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  height: 100%;
}

.row {
  display: flex;
  justify-content: flex-start;
  align-items: stretch;
}

@media (max-width: 768px) {
  .row {
    flex-direction: column;
    align-items: center;
    text-align: center;
  }

  .col-md-4 {
    width: 100%;
    display: flex;
    flex-direction: row;
    justify-content: center;
    gap: 10px;
  }

  .col-md-4 img {
    width: 48%;
  }

  .col-md-8 {
    width: 100%;
    padding: 0 15px;
  }

  .title-with-divider {
    font-size: 1.8rem;
  }

  .custom-text {
    font-size: 1rem;
  }

  .first-paragraph {
    font-size: 1rem;
  }

  .pencil-divider {
    width: 150px;
  }

  .btn {
    width: 100%;
    font-size: 1rem;
  }
}

@media (max-width: 480px) {
  .col-md-4 {
    flex-direction: column;
    align-items: center;
  }

  .col-md-4 img {
    width: 100%;
  }

  .title-with-divider {
    font-size: 1.5rem;
  }

  .custom-text {
    font-size: 0.95rem;
  }

  .first-paragraph {
    font-size: 0.9rem;
  }

  .pencil-divider {
    width: 120px;
  }

  .btn {
    font-size: 0.9rem;
  }
}
</style>
