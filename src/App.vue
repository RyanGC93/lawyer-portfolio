<template>
  <div id="app">
    <NavbarComponent />
    <HeroComponent />
    <AboutComponent />
    <ServicesComponent />
    <TeamComponent />
    <ContactComponent />
    <FooterComponent />
  </div>
</template>

<script>
import NavbarComponent from './components/NavbarComponent.vue';
import HeroComponent from './components/HeroComponent.vue';
import ServicesComponent from './components/ServicesComponent.vue';
import AboutComponent from './components/AboutComponent.vue';
import TeamComponent from './components/TeamComponent.vue';
import ContactComponent from './components/ContactComponent.vue';
import FooterComponent from './components/FooterComponent.vue';

export default {
  name: 'App',
  components: {
    NavbarComponent,
    HeroComponent,
    AboutComponent,
    ServicesComponent,
    TeamComponent,
    ContactComponent,
    FooterComponent,
  },
};
</script>

<style>
body {
  margin: 0;
  font-family: 'Roboto', sans-serif;
}
</style>
