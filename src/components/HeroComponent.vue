<template>
  <section id="hero" class="hero">
    <div class="hero-content">
      <h1>Your Trusted Legal Partner</h1>
      <p>Expert legal services you can rely on</p>
      <a href="#contact" class="cta-btn">Get in Touch</a>
    </div>
  </section>
</template>

<script>
export default {
  name: 'Hero',
};
</script>

<style scoped>
.hero {
  background: url('@/assets/lawyer.jpg') no-repeat center center/cover;
  height: 100vh;
  display: flex;
  align-items: center;
  justify-content: center;
  text-align: center;
  color: #fff;
}
.hero-content {
  background: rgba(0, 0, 0, 0.5);
  padding: 20px;
  border-radius: 10px;
}
.cta-btn {
  background-color: #007bff;
  color: #fff;
  padding: 10px 20px;
  text-decoration: none;
  border-radius: 5px;
  margin-top: 20px;
  display: inline-block;
}
.cta-btn:hover {
  background-color: #0056b3;
}
</style>
