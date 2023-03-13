<script>
export default {

}
</script>

<template>
  <!-- Inizio Hero -->
  <div class="container">
    <div class="hero">
      <span class="title">Contemporary Ideas</span>
      <p>Lorem ipsum dolor sit amet consectetur adipisicing elit.
        Voluptatum minima necessitatibus expedita ratione harum magni dolore quia blanditiis nulla culpa reiciendis
        soluta recusandae exercitationem iusto,
        assumenda veniam molestiae maxime quos.
      </p>
      <div class="button">Register Now</div>
    </div>
  </div>

  <!-- Fine Hero -->
</template>

<style lang="scss" scoped>
@use '../style/partials/variables' as *;

//1 - Importo Font Google
@import url('https://fonts.googleapis.com/css2?family=Merriweather:wght@700&display=swap');
//2 - Creo Variabile con Font importato
$font-merriweather: 'Merriweather', serif;

.hero {
  display: flex;
  gap: 20px;
  flex-direction: column;
  align-items: center;
  font-family: "Open Sans", sans-serif;
  padding: 150px 30px;

  .title {
    font-family: $font-merriweather;
    font-size: 63px;
  }

  p {
    font-size: 16px;
    line-height: 30px;
    text-align: center;
  }

  .button {
    text-transform: uppercase;
    font-size: 14px;
    font-weight: 700;
    padding: 20px 30px;
    background-color: $light-blue;
  }
}
</style>