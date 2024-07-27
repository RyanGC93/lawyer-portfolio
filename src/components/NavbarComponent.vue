<template>
  <nav class="navbar">
    <div class="container">
      <div class="logo">Lawyer</div>
      <div class="nav-links">
        <a href="#hero">Home</a>
        <a href="#services">Services</a>
        <a href="#about">About</a>
        <a href="#contact">Contact</a>
      </div>
    </div>
  </nav>
</template>

<script>
export default {
  name: 'NavbarComponent',
};
</script>

<style scoped>
.navbar {
  background-color: #333;
  color: #fff;
  padding: 15px 0;
  position: fixed;
  width: 100%;
  z-index: 1000;
}
.container {
  display: flex;
  justify-content: space-between;
  align-items: center;
  max-width: 1200px;
  margin: 0 auto;
  padding: 0 20px;
}
.logo {
  font-size: 24px;
  font-weight: bold;
}
.nav-links a {
  margin-left: 20px;
  color: #fff;
  text-decoration: none;
}
.nav-links a:hover {
  color: #ddd;
}
</style>
