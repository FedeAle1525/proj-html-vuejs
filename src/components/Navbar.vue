<script>
export default {

  props: {

    items: {
      type: Array,
      required: true
    }

  }
}
</script>

<template>
  <!-- Inizio NavBar -->
  <div class="container">
    <nav>
      <img class="logo" src="/image/logo-light.png" alt="">

      <div class="menu">
        <ul class="links">
          <li v-for="item in items"> {{ item }}</li>
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
</template>

<style lang="scss" scoped>
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
    font-weight: 400;

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