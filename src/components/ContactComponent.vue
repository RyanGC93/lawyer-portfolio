<template>
  <section id="contact" class="contact">
    <h2>Contact Us</h2>
    <form @submit.prevent="submitForm">
      <input type="text" v-model="name" placeholder="Your Name" required>
      <input type="email" v-model="email" placeholder="Your Email" required>
      <textarea v-model="message" placeholder="Your Message" required></textarea>
      <button type="submit">Send Message</button>
    </form>
  </section>
</template>

<script>
export default {
  name: 'Contact',
  data() {
    return {
      name: '',
      email: '',
      message: '',
    };
  },
  methods: {
    submitForm() {
      alert(`Message sent by ${this.name}`);
      // Implement actual form submission logic here
    },
  },
};
</script>

<style scoped>
.contact {
  padding: 100px 20px;
  text-align: center;
}
form {
  max-width: 600px;
  margin: 0 auto;
  display: flex;
  flex-direction: column;
}
input, textarea {
  margin-bottom: 15px;
  padding: 10px;
  border: 1px solid #ccc;
  border-radius: 5px;
}
button {
  background-color: #007bff;
  color: #fff;
  padding: 10px 20px;
  border: none;
  border-radius: 5px;
  cursor: pointer;
}
button:hover {
  background-color: #0056b3;
}
</style>
