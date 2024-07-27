<template>
  <section id="team" class="team">
    <h2>Our Team</h2>
    <div class="team-container">
      <div class="team-member" v-for="(member, index) in team" :key="index">
        <img :src="member.image" :alt="member.name">
        <h3>{{ member.name }}</h3>
        <p>{{ member.description }}</p>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: 'TeamComponent',
  data() {
    return {
      team: [
        {
          image: require('@/assets/team1.jpg'),
          name: 'John Doe',
          description: 'Senior Partner with over 20 years of experience in corporate law.'
        },
        {
          image: require('@/assets/team2.jpg'),
          name: 'Jane Smith',
          description: 'Expert in family law, committed to helping clients through difficult times.'
        },
        {
          image: require('@/assets/team3.jpg'),
          name: 'Robert Brown',
          description: 'Criminal defense attorney with a proven track record of successful cases.'
        },
        // Add more team members as needed
      ],
    };
  },
};
</script>

<style scoped>
.team {
  padding: 100px 20px;
  text-align: center;
  background-color: #fff;
}
.team-container {
  display: flex;
  justify-content: center;
  flex-wrap: wrap;
}
.team-member {
  background: #f9f9f9;
  margin: 20px;
  padding: 20px;
  border-radius: 10px;
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
  max-width: 300px;
  text-align: left;
}
.team-member img {
  width: 100%;
  border-radius: 10px 10px 0 0;
}
.team-member h3 {
  margin: 15px 0 10px;
}
</style>
