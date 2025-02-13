<script setup>
const urlLogo = "https://le-cdn.hibuwebsites.com/be04dc16d67f484bbb4edb2b6e8fdff9/dms3rep/multi/opt/vintage-outdoor-inc-logo-300w.png";

const navItems = [
  { name: "Home", link: "#" },
  { name: "About Us", link: "#" },
  { name: "Services", link: "#" },
  { name: "Vintage Construction", link: "#" },
  { name: "Gallery", link: "#" },
  { name: "Testimonials", link: "#" },
  { name: "Blog", link: "#" },
  { name: "FAQS", link: "#" },
];
</script>

<template>
  <header>
    <nav class="navbar navbar-expand-lg navbar-light">
      <div class="container-fluid d-flex justify-content-between align-items-center">
        <a class="navbar-brand d-flex align-items-center" href="#">
          <img :src="urlLogo" alt="Logo" width="80" height="50" class="d-inline-block align-text-top">
        </a>
        <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav"
          aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
          <span class="navbar-toggler-icon"></span>
        </button>

        <div class="collapse navbar-collapse" id="navbarNav">
          <ul class="navbar-nav me-auto">
            <li v-for="(item, index) in navItems" :key="index" class="nav-item">
              <a class="nav-link" :href="item.link">{{ item.name }}</a>
            </li>
            <li class="nav-item">
              <button type="button" class="btn btn-warning text-white">Contact Us</button>
            </li>
          </ul>
        </div>
      </div>
    </nav>
  </header>
</template>


<style>
.btn-warning {
  background-color: #C49326;
  border-color: #C49326;
  color: white;
}

.btn-warning:hover {
  background-color: #e0a800;
  border-color: #e0a800;
}

.navbar {
  background-color: transparent !important;
}
</style>
