<template>
  <div>
    <Navbar />
    <!-- MAIN CONTENT -->
    <main>
      <p class="description">
        Welcome to Coder Trader, your go-to platform for all things coding and trading. 
        Explore our resources, tutorials, and community to enhance your skills and knowledge.
        Whether you're a beginner or an experienced coder, we have something for everyone.
        Join us on this exciting journey of learning and growth!
      </p>

      <!-- BIG LOGO IMAGE -->
      <img src="/src/assets/coderTrader.png" alt="Vue Logo" class="logo" />
    </main>
  </div>
</template>

<script lang="ts">
import Navbar from './components/Navbar.vue';
export default {
  name: "App",
  components: {
    Navbar,
  },
};
</script>

<!-- Basic styling to make things look neat -->
<style>
body {
  margin: 0;
  padding: 0;
  font-family: sans-serif;
}

/* NAVBAR */
.navbar {
  background: #eee;
  padding: 1rem;
}

.navbar ul {
  list-style-type: none;
  display: flex;
  gap: 1rem;
  margin: 0;
  padding: 0;
}

.navbar a {
  text-decoration: none;
  color: #333;
}

/* DROPDOWN */
.links-dropdown {
  position: relative;
}

.dropdown-content {
  display: none;
  position: absolute;
  margin-top: 0.5rem;
  list-style: none;
  padding: 0.5rem;
  background: #fff;
  border: 1px solid #ccc;
}

.links-dropdown:hover .dropdown-content {
  display: block;
}

.dropdown-content li {
  margin: 0.5rem 0;
}

/* MAIN CONTENT */
main {
  text-align: center;
  padding: 2rem;
}

.title {
  font-size: 2rem;
  margin-bottom: 1rem;
}

.description {
  font-size: 1.2rem;
  margin-bottom: 2rem;
  max-width: 600px;
  margin: 0 auto 2rem;
}

/* LOGO IMAGE */
.logo {
  width: 200px;
  height: auto;
}
</style>
