<script>
export default {
  data() {
    return {
      cards: [
        {
          img: '/image/h5-custom-icon-1.png',
          type: 'Lenguages'
        },
        {
          img: '/image/h5-custom-icon-2.png',
          type: 'Sotfware'
        },
        {
          img: '/image/h5-custom-icon-3.png',
          type: 'Business'
        },
        {
          img: '/image/h5-custom-icon-4.png',
          type: 'Chemistry'
        },
        {
          img: '/image/h5-custom-icon-5.png',
          type: 'Science'
        },
        {
          img: '/image/h5-custom-icon-6.png',
          type: 'DIY&Craft'
        },
      ]
    }
  }
}
</script>

<template>
  <section>
    <div class="container">
      <div class="row">
        <div class="col-2" v-for="card in cards">
          <div class="card">
            <img :src="card.img">

            <span>{{ card.type }}</span>
          </div>
        </div>
      </div>
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
  padding: 50px 0;
}

.row {
  display: flex;
  margin: 0 -10px;

  .col-2 {
    flex-basis: calc(100% / 6);
    padding: 0 10px;

    .card {
      display: flex;
      flex-direction: column;
      align-items: center;
      padding: 60px 5px;
      gap: 20px;
      background-color: $bg-card-types;

      span {
        font-family: $font-merriweather;
        font-weight: 700;
        font-size: 16px;
      }
    }
  }
}
</style>