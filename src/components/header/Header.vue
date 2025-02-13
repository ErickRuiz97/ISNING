<script setup>
const urlLogo = "https://le-cdn.hibuwebsites.com/be04dc16d67f484bbb4edb2b6e8fdff9/dms3rep/multi/opt/vintage-outdoor-inc-logo-300w.png";
</script>

<template>
  <header>
    <nav class="navbar navbar-expand-lg navbar-light">
      <div class="container-fluid">
        <a class="navbar-brand d-flex align-items-center" href="#">
          <img :src="urlLogo" alt="Logo" width="80" height="50" class="d-inline-block align-text-top">
        </a>
        <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav"
          aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
          <span class="navbar-toggler-icon"></span>
        </button>

        <div class="collapse navbar-collapse" id="navbarNav">
          <ul class="navbar-nav mx-auto">
            <li class="nav-item">
              <a class="nav-link active" href="#">Home</a>
            </li>
            <li class="nav-item">
              <a class="nav-link" href="#">About Us</a>
            </li>
            <li class="nav-item">
              <a class="nav-link" href="#">Services</a>
            </li>
            <li class="nav-item">
              <a class="nav-link" href="#">Vintage Construction</a>
            </li>
            <li class="nav-item">
              <a class="nav-link" href="#">Gallery</a>
            </li>
            <li class="nav-item">
              <a class="nav-link" href="#">Testimonials</a>
            </li>
            <li class="nav-item">
              <a class="nav-link" href="#">Blog</a>
            </li>
            <li class="nav-item">
              <a class="nav-link" href="#">FAQS</a>
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
