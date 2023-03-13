<script>
export default {

  data() {
    return {
      menuItems: ['Home', 'Courses', 'Instructors', 'Event', 'Pages', 'Elements'],
    }
  }
}
</script>

<template>
  <header>
    <!-- Inizio NavBar -->
    <div class="container">
      <nav>
        <img class="logo" src="/image/logo-light.png" alt="">

        <div class="menu">
          <ul class="links">
            <li v-for="item in menuItems"> {{ item }}</li>
          </ul>

          <ul class="icons">
            <li><font-awesome-icon icon="fa-solid fa-magnifying-glass" /></li>
            <li><font-awesome-icon icon="fa-solid fa-bag-shopping" /></li>
            <li><font-awesome-icon icon="fa-solid fa-bars" /></li>
          </ul>
        </div>


      </nav>
    </div>
    <!-- Fine NavBar -->

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

nav {
  padding: 20px 0;
  font-family: "Open Sans", sans-serif;
  display: flex;
  justify-content: space-between;
  align-items: center;

  .logo {
    width: 160px;
  }

  .menu {
    display: flex;
    gap: 30px;
    font-size: 15px;
    font-weight: 400px;

    .links {
      display: flex;
      gap: 40px;
      text-transform: uppercase;
    }

    .icons {
      display: flex;
      gap: 20px;
    }
  }
}
</style>