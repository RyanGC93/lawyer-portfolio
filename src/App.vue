<template>
  <div id="app">
    <Navbar />
    <Hero />
    <Services />
    <About />
    <Contact />
    <Footer />
  </div>
</template>

<script>
import Navbar from './components/Navbar.vue';
import Hero from './components/Hero.vue';
import Services from './components/Services.vue';
import About from './components/About.vue';
import Contact from './components/Contact.vue';
import Footer from './components/Footer.vue';

export default {
  name: 'App',
  components: {
    Navbar,
    Hero,
    Services,
    About,
    Contact,
    Footer,
  },
};
</script>

<style>
body {
  margin: 0;
  font-family: 'Roboto', sans-serif;
}
</style>
