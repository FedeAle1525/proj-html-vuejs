<script>
import Navbar from './Navbar.vue';
import Hero from './Hero.vue';

export default {

  data() {
    return {
      menuItems: ['Home', 'Courses', 'Instructors', 'Event', 'Pages', 'Elements'],
    }
  },

  components: {
    Navbar,
    Hero
  }
}
</script>

<template>
  <header>

    <Navbar :items="menuItems" />

    <Hero />

  </header>
</template>

<style lang="scss" scoped>
header {
  color: white;
  background-image: url('/image/course-9-f-img.jpg');
  background-repeat: no-repeat;
  background-size: cover;
  background-position: 50% 55%;
}
</style>