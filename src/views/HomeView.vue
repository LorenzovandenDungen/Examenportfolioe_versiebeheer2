<template>
  <div class="container">
    <header class="header">
      <!-- De logo afbeelding moet worden aangepast aan je eigen logo -->
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
      <!-- Banner content hier. Je zou een achtergrondafbeelding moeten toevoegen -->
      <h1>Website laten maken?</h1>
      <p>Contact</p>
      <button class="main-button">Meer Informatie</button>
    </div>

    <div class="content">
      <!-- Je content blokken hier -->
      <div class="content-block">
        <h2>Contact</h2>
        <p>Omschrijving van hoe contact op te nemen of diensten.</p>
        <button>Contact Opnemen</button>
      </div>
      <div class="content-block">
        <h2>Tarieven</h2>
        <p>Informatie over je prijzen of pakketten.</p>
        <button>Prijzen Bekijken</button>
      </div>
    </div>

    <div class="features">
      <!-- Voeg hier kenmerken of services toe -->
      <div class="feature-block">Kenmerk 1</div>
      <div class="feature-block">Kenmerk 2</div>
    </div>

    <footer class="footer">
      <!-- Footer informatie -->
      Footer
    </footer>
  </div>
</template>

<script>
export default {
  name: 'HomeView',
  // Voeg hier component logica toe als dat nodig is
};
</script>

<style scoped>
.container {
  display: flex;
  flex-direction: column;
  min-height: 100vh;
  /* Pas kleuren en marges aan op basis van je ontwerp */
}

.header {
  background-color: #fff;
  display: flex;
  justify-content: space-between;
  align-items: center;
  /* Voeg padding en andere stijlen toe zoals nodig */
}

  .logo {
    /* Adjust this as necessary */
    width: 150px;
    height: auto;
  }

  .nav {
    display: flex;
    gap: 1rem;
  }

  .main-banner {
    background-color: #FFEB3B;
    display: flex;
    justify-content: center;
    align-items: center;
    padding: 2rem;
    flex-grow: 1;
  }

  .content {
    display: flex;
    justify-content: space-between;
    flex-grow: 2; /* Allows this section to take up more space */
  }

  .content-block {
    display: flex;
    flex-direction: column;
    align-items: center;
    flex-basis: calc(33.333% - 2rem);
    margin: 1rem;
  }

  .image-placeholder {
    width: 100%;
    height: 150px;
    background-color: #ddd;
    margin-bottom: 1rem;
  }

  .text-placeholder {
    width: 100%;
    height: 2rem;
    background-color: #eee;
    margin-bottom: 1rem;
  }

  .features {
    background-color: #90CAF9;
    display: flex;
    justify-content: space-between;
    flex-grow: 1;
  }

  .feature-block {
    background-color: #fff;
    padding: 1rem;
    flex-basis: calc(33.333% - 2rem);
    margin: 1rem;
  }

  .main-button, button {
    background-color: #000;
    color: #fff;
    border: none;
    padding: 0.5rem 1rem;
    cursor: pointer;
  }

  .footer {
    background-color: #757575;
    color: #fff;
    text-align: center;
    padding: 1rem;
    margin-top: auto; /* Pushes footer to the bottom */
  }
  </style>
