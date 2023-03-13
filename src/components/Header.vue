<script>
import Navbar from './Navbar.vue';

export default {

  data() {
    return {
      menuItems: ['Home', 'Courses', 'Instructors', 'Event', 'Pages', 'Elements'],
    }
  },

  components: {
    Navbar
  }
}
</script>

<template>
  <header>

    <Navbar :items="menuItems" />

    <!-- Inizio Hero -->
    <div class="hero">

    </div>
    <!-- Fine Hiro -->




  </header>
</template>

<style lang="scss" scoped>
header {
  color: white;
  background-image: url('/image/course-9-f-img.jpg');
  background-repeat: no-repeat;
  background-size: cover;
}
</style>