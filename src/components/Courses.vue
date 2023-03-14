<script>

export default {

}

</script>


<template>
  <section>
    <div class="container-small">
      <span>Popular Online Courses</span>
      <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Culpa in similique numquam nostrum veniam possimus,
        ratione fugiat! Modi cumque sapiente sint aperiam,
      </p>
    </div>

    <div class="container">
      <div class="row">
        <div class="col-4">
          <div class="card">
            <div class="card-img">
              <img src="/image/course-5-f-img.jpg">
            </div>

            <div class="card-text">
              <div class="text-header">
                <div class="right">
                  <span class="title">Android Developer</span>
                  <span class="teacher">David Sanders</span>
                </div>
                <div class="left">
                  <span class="free">Free</span>
                </div>
              </div>

              <p>Lorem ipsum dolor sit amet,
                Autem eligendi excepturi nisi quia
                Voluptatum itaque nesciunt error explicabo corporis vero,
                eaque voluptates sequi tempore!
              </p>

              <ul>
                <li>
                  <font-awesome-icon icon="fa-solid fa-user" />
                  1
                </li>
                <li>
                  <font-awesome-icon icon="fa-solid fa-tag" />
                  Programming
                </li>
              </ul>
            </div>
          </div>
        </div>

        <div class="col-4">
          <div class="card">
            <div class="card-img">
              <img src="/image/course-6-f-img.jpg">
            </div>

            <div class="card-text">
              <div class="text-header">
                <div class="right">
                  <span class="title">Web Designing</span>
                  <span class="teacher">Jennifer Powell</span>
                </div>
                <div class="left">
                  <span class="free">Free</span>
                </div>
              </div>

              <p>Lorem ipsum dolor sit amet,
                Autem eligendi excepturi nisi quia
                Voluptatum itaque nesciunt error explicabo corporis vero,
                eaque voluptates sequi tempore!
              </p>

              <ul>
                <li>
                  <font-awesome-icon icon="fa-solid fa-user" />
                  1
                </li>
                <li>
                  <font-awesome-icon icon="fa-solid fa-tag" />
                  Programming
                </li>
              </ul>
            </div>
          </div>
        </div>

        <div class="col-4">
          <div class="card">
            <div class="card-img">
              <img src="/image/course-12-f-img.jpg">
            </div>

            <div class="card-text">
              <div class="text-header">
                <div class="right">
                  <span class="title">Financial Modeling</span>
                  <span class="teacher">Edward Bowman</span>
                </div>
                <div class="left">
                  <span class="twenty">$20</span>
                </div>
              </div>

              <p>Lorem ipsum dolor sit amet,
                Autem eligendi excepturi nisi quia
                Voluptatum itaque nesciunt error explicabo corporis vero,
                eaque voluptates sequi tempore!
              </p>

              <ul>
                <li>
                  <font-awesome-icon icon="fa-solid fa-user" />
                  1
                </li>
                <li>
                  <font-awesome-icon icon="fa-solid fa-tag" />
                  Business
                </li>
              </ul>
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
  border-top: 1px solid #CECECE;
  border-bottom: 1px solid #CECECE;
  padding: 80px 0;
  background-image: url('/image/background-pattern.jpg');
}

.container-small {
  text-align: center;
  margin-bottom: 80px;

  span {
    font-family: $font-merriweather;
    font-size: 45px;
  }

  p {
    font-family: 'Open Sans', sans-serif;
    font-size: 17px;
    font-weight: 400;
    line-height: 26px;
    color: $text-gray;
    margin-top: 20px;
  }
}

.row {
  display: flex;
  margin: 0 -10px;

  .col-4 {
    flex-basis: calc(100% * 4 / 12);
    padding: 0 10px;
  }
}

.card-text {
  padding: 20px 10px;
  font-family: 'Open Sans', sans-serif;
  font-weight: 400;
  border-bottom: 1px solid #CECECE;
  border-left: 1px solid #CECECE;
  border-right: 1px solid #CECECE;

  .text-header {
    display: flex;
    justify-content: space-between;

    .right {
      display: flex;
      flex-direction: column;
      gap: 10px;

      .title {
        font-family: $font-merriweather;
        font-size: 22px;
      }

      .teacher {
        font-size: 15px;
        color: rgb(185, 185, 185);
      }
    }

    .left>.free {
      display: block;
      text-transform: uppercase;
      font-size: 12px;
      line-height: 26px;
      padding: 0 15px;
      color: white;
      background-color: #FFD740;
      border-radius: 999px;
    }

    .left>.twenty {
      display: block;
      font-size: 15px;
      line-height: 26px;
      padding: 0 20px;
      color: white;
      background-color: $light-blue;
      border-radius: 999px;
    }
  }

  p {
    font-size: 15px;
    line-height: 26px;
    color: $text-light-gray;
    margin: 20px 0;
  }

  ul {
    display: flex;
    gap: 15px;

    li {
      font-size: 12px;
      color: rgb(185, 185, 185);
      text-transform: uppercase;
      display: flex;
      gap: 5px;
    }
  }
}
</style>