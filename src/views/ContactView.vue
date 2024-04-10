<template>
  <div class="contact-view">
    <GlobalHeader />
    
    <div class="contact-content">
      <section class="contact-info">
        <h1>Let's Talk</h1>
        <p>Have some big idea or brand to develop and need help? Then reach out we'd love to hear about your project and provide help</p>
        
        <h2>Email</h2>
        <p>beebs@gmail.com</p>
        
        <h2>Socials</h2>
        <a href="https://instagram.com">Instagram</a>
        <a href="https://twitter.com">Twitter</a>
        <a href="https://facebook.com">Facebook</a>
      </section>

      <form class="contact-form">
        <div class="form-field">
          <label for="name">Name</label>
          <input type="text" id="name">
        </div>

        <div class="form-field">
          <label for="email">Email</label>
          <input type="email" id="email">
        </div>

        <div class="form-field">
          <label for="service">What service are you interested in</label>
          <select id="service">
            <option>Select project type</option>
            <!-- Add more options here -->
          </select>
        </div>

        <div class="form-field">
          <label for="budget">Budget</label>
          <select id="budget">
            <option>Select project budget</option>
            <!-- Add more options here -->
          </select>
        </div>

        <div class="form-field">
          <label for="message">Message</label>
          <textarea id="message"></textarea>
        </div>

        <button type="submit">Submit</button>
      </form>
    </div>
  </div>
</template>

<script setup>
import GlobalHeader from '../components/GlobalHeader.vue'
</script>

<style scoped>
.contact-view {
  display: flex;
  flex-direction: column;
}

.contact-content {
  display: flex;
  margin-top: 20px;
}

.contact-info {
  flex: 1;
  padding: 20px;
}

.contact-form {
  flex: 1;
  padding: 20px;
}

.form-field {
  margin-bottom: 20px;
}

.form-field label {
  display: block;
  margin-bottom: 5px;
}

.form-field input[type="text"],
.form-field input[type="email"],
.form-field select,
.form-field textarea {
  width: 100%;
  padding: 10px;
  margin-bottom: 10px;
}

.form-field textarea {
  height: 100px;
}

button[type="submit"] {
  padding: 10px 20px;
  background-color: black;
  color: white;
  border: none;
  cursor: pointer;
}

button[type="submit"]:hover {
  background-color: #333;
}

/* Add additional styling as needed to match the wireframe */
</style>
