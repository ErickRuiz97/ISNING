<script setup>
import Header from "./components/header/Header.vue";
import CardImageTop from "./components/card/CardImageTop.vue";
import CardServices from "./components/card/CardServices.vue";
import CardTestimonial from "./components/card/CardTestimonial.vue";
import CardMain from "./components/card/CardMain.vue";
import WelcomeVintage from "./components/card/WelcomeVintage.vue";
import CardGallery from "./components/card/CardGallery.vue";
import ContactUs from "./components/card/ContactUs.vue";
import FormMessage from "./components/message/FormMessage.vue";
import FootSection from "./components/foot/FootSection.vue";

const imageUrls = {
  piscinaDescanso: "https://www.hotelvinasqueirolo.com/v02/images/piscina-descanso.jpg",
  landscaping: "https://media.istockphoto.com/id/1467596838/photo/residential-garden-landscaping-design-idea.jpg?s=612x612&w=0&k=20&c=qZVvr9oR3a8ZhWoV4TKYJHWgHemPMs17yWUUXsISFe4=",
  vintageConstruction: "https://media.istockphoto.com/id/153006412/es/foto/cascada-de-hidromasaje-y-jacuzzi-en-acci%C3%B3n.jpg?s=612x612&w=0&k=20&c=babqgLo5H_urClHKrNinm48aI1GMWf3uUFC67yOj7qA=",
  testimonialImage1: "https://media.istockphoto.com/id/1310814041/es/foto/retrato-de-una-empresaria-de-pie-en-una-oficina-moderna.jpg?s=612x612&w=0&k=20&c=-_755mSpd6CyF6u5d8khYVwPze5V-FZ_aA6rC90Ye7Y=",
  testimonialImage2: "https://media.istockphoto.com/id/1398994132/es/foto/feliz-mujer-de-negocios-usando-una-tableta-digital-joven-empresaria-l%C3%ADder-que-usa-una-tableta.jpg?s=612x612&w=0&k=20&c=TtzgqiP6O7SHbRgkhzoStGrMA19nXCfcbB8pQCByUBI=",
  playIcon: "https://cdn-icons-png.flaticon.com/512/0/375.png",
  blogImage1: "https://bsrengineering.com/wp-content/uploads/2021/09/DSC_8658.jpg",
  blogImage2: "https://previews.123rf.com/images/traviswolfe/traviswolfe1612/traviswolfe161200062/68783333-vegetaci%C3%B3n-exuberante-selva-cerca-de-la-piscina-en-el-sol-de-la-ma%C3%B1ana-con-los-rayos-c%C3%A1lidos-de.jpg",
  blogImage3: "https://thumbs.dreamstime.com/b/puesta-de-sol-junto-la-piscina-un-momento-m%C3%A1gico-reflejado-en-una-cristalina-decoraci%C3%B3n-fondo-escritorio-portada-del-folleto-325561924.jpg"
};

const serviceDetails = {
  outdoorLiving: "Patios & Decks: Custom outdoor patios and decks. Outdoor Kitchens: Gourmet kitchens for outdoor dining. Pools & Water Features: Stunning pools and waterfalls. FirePits & Heating: Cozy fire pits and heaters. Landscape Lighting: Professional outdoor lighting. Solar Panels: Eco-friendly solar installations.",
  landscapingServices: "Design & Installation: Expert landscape design and setup. Garden Maintenance: Ongoing garden care. Irrigation Systems: Efficient watering solutions. Tree Care: Professional tree maintenance.",
  vintageConstruction: "New Construction: Custom homes and buildings. Remodels: Expert home and business renovations. ADUs: Accessory Dwelling Units for extra space. Investment Properties: Quality construction for investors. Commercial Projects: Tailored business construction."
};
</script>

<template>
  <header>
    <Header />
  </header>
  <main>
    <div class="card-container">
      <CardMain />
    </div>
    <div class="card-container">
      <WelcomeVintage />
    </div>
    <h1 class="display-5 title-with-divider">Our Services</h1>
    <div class="pencil-divider"></div>
    <div class="card-container">
      <CardServices :imageSrc="imageUrls.piscinaDescanso" title="Outdoor Living Spaces"
        :details="serviceDetails.outdoorLiving" :iconSrc="imageUrls.playIcon" />
      <CardServices :imageSrc="imageUrls.landscaping" title="Landscaping Services"
        :details="serviceDetails.landscapingServices" :iconSrc="imageUrls.playIcon" />
      <CardServices :imageSrc="imageUrls.vintageConstruction" title="Vintage Construction Inc"
        :details="serviceDetails.vintageConstruction" :iconSrc="imageUrls.playIcon" />
    </div>

    <div class="card-container">
      <CardGallery />
    </div>
    <h1 class="display-5 title-with-divider">Testimonials</h1>
    <div class="pencil-divider"></div>
    <p class="description">
      Don't just take our word for it-hear from our satisfied clients! We take pride in the strong relationships we've
      built with our clients, and their feedback speaks to our commitment to excellence.
    </p>
    <div class="card-container">
      <CardTestimonial :name="'Laura Chen'"
        :text="'Their attention to detail and professionalism exceeded our expectations. Highly recommend.'"
        :imageSrc="imageUrls.testimonialImage1" :playIcon="imageUrls.playIcon" />
      <CardTestimonial :name="'Laura Chen'"
        :text="'Their attention to detail and professionalism exceeded our expectations. Highly recommend.'"
        :imageSrc="imageUrls.testimonialImage2" :playIcon="imageUrls.playIcon" />
    </div>

    <h1 class="display-5 title-with-divider">Our Blog</h1>
    <p class="description">
      Whether you're looking for expert advice, project inspiration, or updates on our recent work, you'll find it all
      here. Explore our articles to stay informed and inspired!
    </p>
    <div class="card-container mb-4">
      <CardImageTop :imageSrc="imageUrls.blogImage1" :title="'The Ultimate Guide to Home Remodeling'"
        :subtitle="'Trends and Tips'" />
      <CardImageTop :imageSrc="imageUrls.blogImage2" :title="'Transform Your Outdoor Space'"
        :subtitle="'5 Essential Tips'" />
      <CardImageTop :imageSrc="imageUrls.blogImage3" :title="'Sustainable Landscaping'"
        :subtitle="'Eco-Friendly Practices'" />
    </div>
    <button class="btn discover">
      Discover More
    </button>
    <ContactUs />
    <FormMessage />
    <FootSection />
  </main>
</template>

<style scoped>
.discover {
  background-color: #C49326;
  color: white;
  display: block;
  width: auto;
  max-width: 250px;
  margin: 250px auto;
  margin-top: 100px !important;
  font-size: 1.1rem;
  padding: 15px 60px;
  border-radius: 25px;
  font-weight: bold;
  text-align: center;
}


.description {
  text-align: center;
  font-size: 1rem;
  color: #555;
  width: 50%;
  margin: 0 auto;
  margin-bottom: 10px;
}

.display-5 {
  font-weight: 400;
  position: relative;
  text-align: center;
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

.card-container {
  display: flex;
  justify-content: space-between;
  gap: 40px;
  margin-bottom: 30px;
}

.card-container .custom-card {
  flex: 1;
}
</style>
