<script>
import Menus from './Menus.vue';
import Credits from './Credits.vue';

export default {

  components: {
    Menus,
    Credits
  }
}
</script>

<template>
  <footer>
    <Menus />

    <Credits />
  </footer>
</template>


<style lang="scss" scoped>
footer {
  background-color: #222222;
}
</style>

