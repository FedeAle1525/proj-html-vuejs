<script>
export default {
  data() {
    return {
      infos: ['What We Do', 'Degree Programme', 'Career Achievements',
        'Personal Menagment', 'Steps To Success', 'Knowledge Transfer']
    }
  }
}
</script>


<template>
  <section>
    <div class="container">
      <div class="row">
        <div class="col-4">
          <div class="info" v-for="info in infos">
            {{ info }}
          </div>
        </div>
        <div class="col-8">
          <span>Learning Possibilities</span>

          <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Magni deserunt consequuntur eligendi
            nam nisi numquam praesentium minima maxime cupiditate, incidunt, eum quia aliquam minus
            doloremque natus ex assumenda temporibus laboriosam.
          </p>

          <div class="bottom">
            <ul>
              <li>
                <font-awesome-icon icon="fa-solid fa-check" class="icon" />
                We enrich lives through learning.
              </li>
              <li>
                <font-awesome-icon icon="fa-solid fa-check" class="icon" />
                Miximizing potential through individual attention.
              </li>
              <li>
                <font-awesome-icon icon="fa-solid fa-check" class="icon" />
                The trusted name for specialized training.
              </li>
              <li>
                <font-awesome-icon icon="fa-solid fa-check" class="icon" />
                People teach. People learn. This is where they connect.
              </li>
            </ul>

            <img src="/image/h12-tabs-icon-1.png">
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
  padding: 80px 0;
}

.row {
  display: flex;
  margin: 0 -20px;

  .col-4 {
    flex-basis: calc(100% * 4 / 12);
    padding: 0 20px;
  }

  .col-8 {
    flex-basis: calc(100% * 8 / 12);
    padding: 0 20px;
    font-family: 'Open Sans', sans-serif;
    display: flex;
    flex-direction: column;
    gap: 20px;

    span {
      font-family: $font-merriweather;
      font-size: 37px;
    }

    p {
      font-size: 17px;
      line-height: 28px;
      color: $text-light-gray;
      margin-bottom: 20px;
    }

    ul {
      display: flex;
      flex-direction: column;
      gap: 25px;

      li {
        font-size: 15px;
        color: $text-light-gray;

        .icon {
          color: $light-blue;
          margin-right: 5px;
        }

      }
    }
  }
}

.bottom {
  display: flex;
  justify-content: space-between;

  img {
    max-width: 20%;
  }
}

.info {
  color: rgb(132, 123, 123);
  font-family: $font-merriweather;
  font-size: 16px;
  border-top: 1px solid #CECECE;
  border-left: 1px solid #CECECE;
  border-right: 1px solid #CECECE;
  padding: 20px 0 20px 20px;

  // &::before {
  //   content: '';
  //   display: block;
  //   height: 100%;
  //   width: 2px;
  //   background-color: $light-blue;

  // }

  &:hover {
    background-color: #F2F2F2;
    color: $light-blue;
    cursor: pointer;
  }

  &:last-child {
    border-bottom: 1px solid #CECECE;
  }

}
</style>