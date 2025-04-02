<template>
  <nav class="navbar">
    <div class="container">
      <a href="/" class="logo">CoderTrader</a>
      <ul class="nav-links">
        <li><a href="https://www.skool.com/codertrader">skool</a></li>
        <li><a href="https://www.youtube.com/@CoderTrader-j7t">YouTube</a></li>
      </ul>
    </div>
  </nav>
</template>

<script lang="ts">
export default {
  name: "Navbar",
};
</script>

<style scoped>
.navbar {
  background-color: #333;
  color: white;
  padding: 1rem 0;
}

.container {
  display: flex;
  justify-content: space-between;
  align-items: center;
  max-width: 1200px;
  margin: 0 auto;
  padding: 0 1rem;
}

.logo {
  font-size: 1.5rem;
  font-weight: bold;
  text-decoration: none;
  color: white;
}

.nav-links {
  list-style: none;
  display: flex;
  gap: 1.5rem;
  margin: 0;
  padding: 0;
}

.nav-links a {
  text-decoration: none;
  color: white;
  font-size: 1rem;
  transition: color 0.3s;
}

.nav-links a:hover {
  color: #00bcd4;
}
</style>