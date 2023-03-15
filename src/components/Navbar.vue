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
          <li class="icon-bag">
            <font-awesome-icon icon="fa-solid fa-bag-shopping" />
            <div class="label">0</div>
          </li>
          <li><font-awesome-icon icon="fa-solid fa-bars" /></li>
        </ul>
      </div>

    </nav>
  </div>
  <!-- Fine NavBar -->
</template>

<style lang="scss" scoped>
@use '../style/partials/variables' as *;

.icon-bag {
  position: relative;
}

.label {
  display: flex;
  align-items: center;
  justify-content: center;
  width: 15px;
  aspect-ratio: 1/1;
  border-radius: 50%;
  background-color: $light-blue;
  color: white;
  font-size: 10px;
  position: absolute;
  top: 0;
  right: 0;
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
    font-weight: 400;

    .links {
      display: flex;
      gap: 40px;
      text-transform: uppercase;

      li {
        padding: 5px;
        font-weight: 600;
      }

      li:hover {
        color: $light-blue;
        cursor: pointer;
        background: $bg-card-types;
      }
    }

    .icons {
      display: flex;
      gap: 20px;

      li {
        font-size: 20px;
        padding: 0 5px;
      }

      li:hover {
        color: $light-blue;
        cursor: pointer;
      }


    }
  }
}
</style>