<template>
  <section id="about" class="about">
    <h2>About Us</h2>
    <p>
      We are a dedicated team of legal professionals committed to providing top-notch legal services. Our mission is to ensure our clients receive the best possible legal representation and advice.
    </p>
    <p>
      <strong>Our New York Office:</strong><br>
      123 Legal Street,<br>
      Suite 456,<br>
      New York, NY 10001
    </p>
  </section>
</template>

<script>
export default {
  name: 'AboutComponent',
};
</script>

<style scoped>
.about {
  padding: 100px 20px;
  text-align: center;
}
.about p {
  max-width: 800px;
  margin: 0 auto;
  margin-bottom: 20px; /* Add margin between paragraphs */
}
</style>
