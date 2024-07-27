<template>
  <section id="services" class="services">
    <h2>Our Services</h2>
    <div class="services-container">
      <div class="service-card" v-for="(service, index) in services" :key="index">
        <img :src="service.image" :alt="service.title">
        <h3>{{ service.title }}</h3>
        <p>{{ service.description }}</p>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: 'ServicesComponent',
  data() {
    return {
      services: [
        {
          image: require('@/assets/service1.jpg'),
          title: 'Corporate Law',
          description: 'Expert advice on corporate legal matters.'
        },
        {
          image: require('@/assets/service2.jpg'),
          title: 'Family Law',
          description: 'Compassionate and effective family law services.'
        },
        {
          image: require('@/assets/service3.jpg'),
          title: 'Criminal Law',
          description: 'Strong defense for criminal charges.'
        },
        // Add more services as needed
      ],
    };
  },
};
</script>

<style scoped>
.services {
  padding: 100px 20px;
  background-color: #f9f9f9;
  text-align: center;
}
.services-container {
  display: flex;
  justify-content: center;
  flex-wrap: wrap;
}
.service-card {
  background: #fff;
  margin: 20px;
  padding: 20px;
  border-radius: 10px;
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
  max-width: 300px;
  text-align: left;
}
.service-card img {
  width: 100%;
  border-radius: 10px 10px 0 0;
}
.service-card h3 {
  margin: 15px 0 10px;
}
</style>
