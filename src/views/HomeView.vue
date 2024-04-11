<template>
  <div class="container-fluid"> <!-- Use container-fluid for full width -->
    <!-- Bootstrap Navbar or Header -->
    <header class="mb-5"> <!-- Added margin bottom -->
      <nav class="navbar navbar-expand-lg navbar-light bg-light">
        <router-link class="navbar-brand" to="/">Lorenzo</router-link>
      </nav>
    </header>

    <!-- Main Banner with Background Image -->
    <div class="main-banner text-white text-center py-5 mb-5"> <!-- Added margin bottom -->
      <h1 class="banner-title display-3">Website laten maken?</h1>
      <button class="btn btn-secondary" @click="navigateTo('/contact')">Contact</button>
    </div>

    <!-- Content Section -->
    <div class="row"> <!-- Use row for a grid layout -->
      <div v-for="block in blocks" :key="block.title" class="col-md-4 mb-5"> <!-- Use col-md-4 to take up 4/12 of the container width for each block, added margin bottom -->
        <div class="image-block bg-primary mb-3" style="height: 200px;"></div> <!-- Added inline style for height -->
        <h2 class="block-title h4">{{ block.title }}</h2>
        <p class="block-description">{{ block.description }}</p>
        <button class="btn btn-primary" @click="navigateTo(block.route)">{{ block.buttonText }}</button>
      </div>
    </div>

    <!-- Footer -->
    <footer class="footer bg-dark text-white text-center py-3 mt-auto"> <!-- mt-auto will push the footer to the bottom -->
      &copy; 2024 Your Company Name. All Rights Reserved.
    </footer>
  </div>
</template>

<script>
// Import your image here so Webpack handles it
import mainBannerImage from '@/assets/Foto_main_banner.png';

export default {
  name: 'HomeView',
  data() {
    return {
      // ... your data properties ...
      mainBannerImageUrl: mainBannerImage // This will be used in the style below
    };
  },
  methods: {
    navigateTo(route) {
      this.$router.push(route);
    }
  }
};
</script>

<style scoped>
.main-banner {
  background-image: url('../assets/Foto_main_banner.png'); /* Webpack will resolve this URL */
  background-size: cover;
  background-position: center;
  min-height: 400px; /* Adjust height as necessary */
}

/* You can remove this if there are no more custom styles or keep it for further customizations */
</style>
