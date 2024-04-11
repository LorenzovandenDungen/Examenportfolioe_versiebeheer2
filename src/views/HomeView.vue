<template>
  <div class="container">
    <header class="header">

    </header>

    <div class="main-banner">
      <h1 class="banner-title">Website laten maken?</h1>
      <button class="banner-button" @click="navigateTo('/contact')">Contact</button>
    </div>

    <div class="content-section">
      <div v-for="block in blocks" :key="block.title" class="content-block">
        <div class="image-block"></div>
        <h2 class="block-title">{{ block.title }}</h2>
        <p class="block-description">{{ block.description }}</p>
        <button class="block-button" @click="navigateTo(block.route)">{{ block.buttonText }}</button>
      </div>
    </div>

    <footer class="footer">
      &copy; 2024 Your Company Name. All Rights Reserved.
    </footer>
  </div>
</template>

<script>
export default {
  name: 'HomeView',
  data() {
    return {
      navLinks: [
        { to: '/', text: 'Home' },
        { to: '/websites', text: 'Websites' },
        { to: '/tarieven', text: 'Tarieven' },
        { to: '/contact', text: 'Contact' },
        { to: '/offerte', text: 'Offerte' }
      ],
      blocks: [
        { title: 'Contact', description: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit.', route: '/contact', buttonText: 'Meer informatie' },
        { title: 'Tarieven', description: 'Pellentesque habitant morbi tristique senectus et netus.', route: '/tarieven', buttonText: 'Bekijk pakketten' },
        { title: 'Websites', description: 'Sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.', route: '/websites', buttonText: 'Bekijk voorbeelden' }
      ]
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
.container {
  display: flex;
  flex-direction: column;
  min-height: 100vh;
  font-family: 'Arial', sans-serif;
}

.header {
  background-color: #fff;
  padding: 1rem 5%;
  display: flex;
  justify-content: space-between;
  align-items: center;
  box-shadow: 0 2px 4px rgba(0,0,0,0.1);
}

.logo {
  width: auto;
  height: 50px;
}

.nav {
  display: flex;
  gap: 2rem;
  align-items: center;
  list-style-type: none;
  margin: 0;
  padding: 0;
}

.nav-link {
  text-decoration: none;
  color: #333;
  font-weight: bold;
  padding: 0.5rem 1rem;
}

.main-banner {
  background-image: url('./Foto_main_banner.png');
  background-size: cover;
  background-position: center;
  text-align: center;
  padding: 5rem 1rem;
  position: relative;
  color: #fff;
}

.banner-title {
  font-size: 2.5rem;
  margin-bottom: 0.5rem;
}

.banner-button {
  background-color: #000;
  color: #fff;
  border: none;
  padding: 0.75rem 2rem;
  cursor: pointer;
  font-size: 1rem;
}

.content-section {
  display: flex;
  justify-content: space-around;
  padding: 2rem 5%;
}

.content-block {
  width: 30%;
  text-align: center;
}

.image-block {
  background-color: #0d6efd; /* Bootstrap primary color */
  height: 200px;
  margin-bottom: 1rem;
}

.block-title {
  margin-bottom: 0.5rem;
  font-size: 1.25rem;
}

.block-description {
  margin-bottom: 1rem;
  color: #666;
  font-size: 1rem;
}

.block-button {
  background-color: #0d6efd; /* Bootstrap primary color */
  color: #fff;
  border: none;
  padding: 0.5rem 1rem;
  cursor: pointer;
  font-size: 1rem;
}

.footer {
  background-color: #343a40; /* Bootstrap dark */
  color: #fff;
  text-align: center;
  padding: 1rem;
  margin-top: auto;
}
</style>
