<script>
export default {

}
</script>


<template>
  <section>
    <div class="container">
      <div class="row">
        <div class="col-6">
          <img src="/image/h5-img-2.jpg">
        </div>

        <div class="col-6">
          <div class="card">
            <span>Empowering <br> Children to Reach <br> Their Potentials.</span>
            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. <br>
              Hic laboriosam consequuntur nam magni adipisci <br>
              perferendis tempora quas nesciunt, sint doloribus <br>
              officia aut error odit mollitia velit ex, blanditiis non. Qui?
            </p>

            <div class="numbers">
              <div class="data">
                <span class="num">168</span>

                <span class="text">User Stories</span>
              </div>

              <div class="data">
                <span class="num">347</span>

                <span class="text">Events</span>
              </div>
            </div>
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
  padding: 30px 0;
}

.row {
  display: flex;
  margin: 0 -20px;

  .col-6 {
    flex-basis: calc(100% / 2);
    padding: 0 20px;
  }
}

.card {
  display: flex;
  flex-direction: column;
  gap: 20px;

  span {
    font-family: $font-merriweather;
    font-size: 37px;
    line-height: 50px;
  }

  p {
    font-family: 'Open Sans', sans-serif;
    font-weight: 400;
    font-size: 17px;
    line-height: 26px;
    color: $text-gray;
  }

  .numbers {
    display: flex;
    justify-content: start;
    gap: 170px;
    margin-top: 10px;

    .data {
      display: flex;
      flex-direction: column;

      .num {
        font-size: 48px;
        color: $light-blue;
      }

      .text {
        font-size: 18px;
        color: $light-blue;
      }
    }
  }
}
</style>