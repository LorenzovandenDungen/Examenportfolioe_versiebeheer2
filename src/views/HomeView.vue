<template>
  <div class="container">
    <header class="header">
      <img class="logo" src="./Logo.png" alt="Logo">
      <nav class="nav">
        <a href="#home">Home</a>
        <a href="#websites">Websites</a>
        <a href="#tarieven">Tarieven</a>
        <a href="#contact">Contact</a>
        <a href="#offerte">Offerte</a>
      </nav>
    </header>

    <div class="main-banner">
      <div class="banner-content">
        <h1>Website laten maken?</h1>
        <button class="main-button">Contact</button>
      </div>
    </div>

    <div class="content">
      <div class="content-block">
        <div class="title-placeholder"></div>
        <div class="text-placeholder"></div>
        <button>Button</button>
      </div>
      <div class="content-block">
        <div class="title-placeholder"></div>
        <div class="text-placeholder"></div>
        <button>Button</button>
      </div>
      <div class="content-block">
        <div class="title-placeholder"></div>
        <div class="text-placeholder"></div>
        <button>Button</button>
      </div>
    </div>

    <footer class="footer">
      Footer
    </footer>
  </div>
</template>

<script>
export default {
  name: 'HomeView',
};
</script>

<style scoped>
.container {
  display: flex;
  flex-direction: column;
  min-height: 100vh;
}

.header {
  background-color: #fff;
  padding: 1rem 5%;
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.logo {
  width: auto;
  height: 50px; /* Adjust based on your logo's aspect ratio */
}

.nav {
  display: flex;
  gap: 2rem;
  align-items: center;
  list-style-type: none;
  margin: 0;
  padding: 0;
}

.nav a {
  text-decoration: none;
  color: #333;
  font-weight: bold;
}

.main-banner {
  position: relative;
  background-image: url('./Foto_main_banner.png');
  background-size: cover;
  background-position: center;
  padding: 4rem 0;
}

.banner-content {
  width: 100%;
  text-align: center;
}

.content {
  display: flex;
  padding: 2rem 5%;
}

.content-block {
  flex: 1;
  margin: 0 1rem;
  text-align: center;
}

.title-placeholder {
  height: 3rem; /* Title height */
  background-color: #eee; /* Title placeholder color */
  margin-bottom: 1rem;
}

.text-placeholder {
  height: 6rem; /* Text placeholder height */
  background-color: #f5f5f5; /* Text placeholder color */
  margin-bottom: 2rem;
}

.main-button, .content button {
  background-color: #000;
  color: #fff;
  border: none;
  padding: 0.5rem 1rem;
  cursor: pointer;
  margin-top: 1rem;
}

.footer {
  background-color: #757575;
  color: #fff;
  text-align: center;
  padding: 1rem;
  margin-top: auto;
}
</style>
