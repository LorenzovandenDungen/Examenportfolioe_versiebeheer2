<template>
  <div class="tarieven-view">
    <header>
      <!-- Navigation goes here -->
    </header>

    <main class="content">
      <h1 class="title">Tarieven</h1>
      <p class="introduction">Korte inleiding</p>
      <div class="price-container">
        <div class="price-box free">
          <h2>FREE</h2>
          <p class="price">$0/month</p>
          <ul>
            <li>✔ PNG templates</li>
          </ul>
          <button class="buy-button">Probeer nu</button>
        </div>
        <div class="price-box premium">
          <h2>PREMIUM</h2>
          <p class="price">$99/month</p>
          <ul>
            <li>✔ PNG templates</li>
            <li>✔ Figma responsive components</li>
          </ul>
          <button class="buy-button">Probeer nu</button>
        </div>
        <div class="price-box pro">
          <h2>PRO</h2>
          <p class="price">$199/month</p>
          <ul>
            <li>✔ PNG templates</li>
            <li>✔ Figma responsive components</li>
            <li>✔ Constant updates</li>
          </ul>
          <button class="buy-button">Probeer nu</button>
        </div>
      </div>
    </main>

    <footer>
      <p class="footer-content">Footer</p>
    </footer>
  </div>
</template>

<script setup>
// Import your components or any scripts if needed
</script>

<style scoped>
.tarieven-view {
  font-family: 'Arial', sans-serif;
  display: flex;
  flex-direction: column;
  min-height: 100vh;
}

header {
  /* Add header styles here */
}

.content {
  flex: 1;
  text-align: center;
  padding: 40px 20px;
  max-width: 1200px;
  margin: auto;
}

.title {
  margin-bottom: 1em;
}

.introduction {
  font-size: 20px;
  font-weight: bold;
  margin-bottom: 2em;
}

.price-container {
  display: flex;
  justify-content: space-evenly;
  flex-wrap: wrap;
  gap: 30px;
}

.price-box {
  border: 1px solid #ccc;
  padding: 2em;
  width: 300px;
  min-height: 250px; /* Adjust height as necessary */
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  box-shadow: 0 2px 5px rgba(0, 0, 0, 0.2);
}

.price-box h2 {
  margin: 0;
  font-size: 1.25em;
  font-weight: normal;
  text-transform: uppercase;
  color: #333; /* Adjust the color to match the design */
}

.price {
  font-size: 2em; /* Adjust the font size to match the design */
  font-weight: bold;
  margin: 0.5em 0;
}

.price-box ul {
  list-style: none;
  padding: 0;
  margin: 1em 0;
  text-align: left;
}

.price-box li {
  margin-bottom: 0.5em;
  font-size: 1em; /* Adjust the font size to match the design */
}

.buy-button {
  background-color: #4CAF50; /* Adjust the button color to match the design */
  padding: 10px 20px;
  cursor: pointer;
  border: none;
  color: white; /* Text color */
  text-transform: uppercase;
  font-weight: bold;
  transition: background-color 0.3s ease;
}

.buy-button:hover {
  background-color: #45a049; /* Darker shade for hover effect */
}

footer {
  border-top: 1px solid #ccc;
  padding: 1em 0;
  text-align: center;
}

.footer-content {
  margin: 0;
}
</style>
