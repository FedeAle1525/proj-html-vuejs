<script>
export default {

}
</script>


<template>
  <section>
    <div class="container">
      <div class="row">
        <div class="col-3">
          <div class="menu">
            <img class="logo" src="/image/logo-light.png">

            <p>
              Providing Life Changing Experiences Through Education. Class That Fit Your Busy Life. Closer to Home
            </p>

            <div class="phone">
              <font-awesome-icon icon="fa-solid fa-phone" />
              <span>1-677-124-44227</span>
            </div>

            <div class="time">
              <font-awesome-icon icon="fa-regular fa-clock" />
              <span>Mon - Sat 8.00 - 18.00</span>
            </div>

          </div>
        </div>

        <div class="col-3">
          <div class="menu">
            <span class="title">Popular Courses</span>

            <div class="course">
              <span class="name">Business English</span>
              <span class="teacher">Preston Marshall</span>
            </div>

            <div class="course">
              <span class="name">Social Computing</span>
              <span class="teacher">David Sanders</span>
            </div>

            <div class="course">
              <span class="name">Learn Spanish</span>
              <span class="teacher">Jennie King</span>
            </div>
          </div>
        </div>

        <div class="col-3">
          <div class="menu">
            <span class="title">Support</span>

            <ul>
              <li>User Dashboard</li>
              <li>Contact Us</li>
              <li>FAQ</li>
              <li>Course Offer</li>
              <li>Events</li>
            </ul>
          </div>
        </div>

        <div class="col-3">
          <div class="menu">
            <span class="title">Flexible Learning</span>

            <img class="map" src="/image/footer-img-1.png">
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
  font-family: 'Open Sans', sans-serif;
  font-weight: 400;
  color: #CECECE
}

.row {
  display: flex;
  margin: 0 -15px;

  .col-3 {
    flex-basis: calc(100% / 4);
    padding: 0 15px;

    .menu {
      display: flex;
      flex-direction: column;
      gap: 25px;

      .logo {
        width: 140px;
      }

      p {
        font-size: 15px;
        line-height: 26px;
      }

      .phone,
      .time {
        font-size: 12px;
        color: white;

        span {
          margin-left: 10px;
        }
      }

      .title {
        font-family: $font-merriweather;
        font-size: 22px;
        color: white;
      }

      .course {
        display: flex;
        flex-direction: column;
        line-height: 26px;

        .name {
          font-family: $font-merriweather;
          font-size: 16px;

          &:hover {
            color: $light-blue;
            cursor: pointer;
          }
        }

        .teacher {
          font-size: 14px;
        }
      }

      ul {
        display: flex;
        flex-direction: column;
        gap: 20px;

        li {
          font-size: 15px;

          &:hover {
            color: $light-blue;
            cursor: pointer;
          }
        }
      }
    }

  }
}
</style>