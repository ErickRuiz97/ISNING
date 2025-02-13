<template>
  <div class="gallery-section">
    <div class="header">
    </div>
    <div class="content">
      <div class="text-section">
        <h1 class="display-5 title-with-divider">Explore Our Gallery</h1>
        <div class="pencil-divider"></div>
        <p class="description">
          Take a look at our recent projects to see the quality and creativity we bring to every job. Whether it's a
          beautifully landscaped garden or a newly built home, our portfolio showcases the best of what Vintage Outdoor
          Inc. and Vintage Construction Inc. can offer.
        </p>
      </div>
      <div class="images-section">
        <div class="image-group top-row">
          <img
            src="https://phantom-expansion.unidadeditorial.es/33e9a0c7ad9c77e09f8a6ad6b567ecc2/resize/640/assets/multimedia/imagenes/2022/06/21/16558349335252.jpg"
            class="image">
          <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSAhIQ7BlHCUuBrQX06vEkRP39SreEN3CvOwQ&s"
            class="image">
          <img
            src="https://s3.abcstatics.com/abc/www/multimedia/viajar/2024/08/01/asi-gardens-RuIKNI5YOI3l58H75O35uVK-1200x840@diario_abc.jpg"
            class="image">
        </div>
        <div class="image-group bottom-row">
          <img
            src="https://img.freepik.com/fotos-premium/villa-privada-cara-piscina-casa-privada-noche-casa-campo-exterior-mansion_1194258-41262.jpg"
            class="image-bottom">
          <img
            src="https://previews.123rf.com/images/bhakpong/bhakpong1604/bhakpong160400181/55878546-nataci%C3%B3n-piscina-serie-cara-de-la-piscina.jpg"
            class="image-bottom">
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
defineProps({
});
</script>

<style scoped>
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

.display-5 {
  font-weight: 400;
  position: relative;
  display: inline-block;
}

.gallery-section {
  display: flex;
  flex-direction: column;
  padding: 40px;
  background-color: #f4f4f4;
}

.header {
  text-align: center;
  margin-bottom: 30px;
}

.title {
  font-size: 2rem;
  font-weight: bold;
  color: #333;
}

.content {
  display: flex;
  justify-content: space-between;
  gap: 30px;
}

.text-section {
  flex: 1;
  padding-right: 20px;
}

.description {
  font-size: 1rem;
  color: #555;
}

.images-section {
  flex: 2;
  display: flex;
  flex-direction: column;
  gap: 20px;
}

.image-group {
  display: flex;
  gap: 20px;
  justify-content: space-between;
}

.top-row {
  flex: 1;
}

.bottom-row {
  flex: 1;
  justify-content: space-between;
}

.image-bottom {
  width: 55%;
  height: 200px;
  object-fit: cover;
  border-radius: 30px;
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
}

.image {
  width: 32%;
  height: 200px;
  object-fit: cover;
  border-radius: 30px;
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
}

@media (max-width: 768px) {
  .content {
    flex-direction: column;
    align-items: center;
  }

  .text-section {
    padding-right: 0;
    margin-bottom: 20px;
  }

  .images-section {
    flex-direction: column;
    justify-content: center;
  }

  .image-group {
    flex-direction: column;
    align-items: center;
  }

  .image {
    width: 100%;
    height: auto;
  }
}

@media (max-width: 768px) {
  .gallery-section {
    padding: 20px;
  }

  .text-section {
    text-align: center;
  }

  .images-section {
    flex-direction: column;
    justify-content: center;
  }

  .image-group {
    flex-direction: column;
    align-items: center;
    gap: 10px;
  }

  .image {
    width: 100%;
    height: auto;
  }

  .image-bottom {
    width: 100%;
  }
}
</style>
