<script>
import LabelTop from './LabelTop.vue';

export default {

  components: {
    LabelTop,
  }
}
</script>


<template>
  <section>
    <div class="container">
      <span>The Trusted Name <br>
        for In-Home Tutoring.
      </span>

      <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Iure repudiandae fugit rem sint veniam quam doloremque
        dolorum beatae expedita alias ducimus soluta quos, explicabo mollitia quidem quisquam vel pariatur qui.
      </p>

      <a href="#">Learn More</a>

      <img src="/image/h5-img-1.jpg">

      <!-- <LabelTop class="label" /> -->
    </div>
  </section>
</template>


<style lang="scss" scoped>
@use '../style/partials/variables' as *;

//1 - Importo Font Google
@import url('https://fonts.googleapis.com/css2?family=Merriweather:wght@700&display=swap');
//2 - Creo Variabile con Font importato
$font-merriweather: 'Merriweather', serif;

section {
  position: relative;
}

.container {
  padding: 50px 0;
  display: flex;
  flex-direction: column;
  gap: 20px;
  font-family: 'Open Sans', sans-serif;

  span {
    font-family: $font-merriweather;
    font-size: 37px;
  }

  p {
    font-size: 17px;
    font-weight: 400;
    line-height: 26px;
    color: $text-gray;
  }

  a {
    font-size: 14px;
    font-weight: 700;
    text-transform: uppercase;
    color: $light-blue;
  }

  img {
    max-width: 90%;
  }

  .label {
    position: absolute;
    right: 0;
    bottom: 25%;
  }
}
</style>