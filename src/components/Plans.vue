<script>
export default {

}
</script>

<template>
  <section>
    <div class="container-small">
      <span>Pricing Plans</span>
      <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Culpa in similique numquam nostrum veniam.</p>
    </div>

    <div class="container">
      <table>
        <tr class="header">
          <td class="discount">
            Save up to 40% <br> by paying weekly
          </td>
          <td class="plan">
            <ul class="list">
              <li class="img">
                <img src="/image/h5-custom-icon-7.png">
              </li>
              <li class="name">Standard</li>
              <li class="price">$12</li>
            </ul>
          </td>
          <td class="plan">
            <ul class="list">
              <li class="img">
                <img src="/image/h5-custom-icon-8.png">
              </li>
              <li class="name">Professional</li>
              <li class="price">$59</li>
            </ul>
          </td>
          <td class="plan">
            <ul class="list">
              <li class="img">
                <img src="/image/h5-custom-icon-9.png">
              </li>
              <li class="name">Advance</li>
              <li class="price">$88</li>
            </ul>
          </td>
        </tr>

        <tr class="info">
          <td class="title">Number Of Courses</td>
          <td>2</td>
          <td>4</td>
          <td>6</td>
        </tr>

        <tr class="info">
          <td class="title">Time</td>
          <td>15 days</td>
          <td>30 Days</td>
          <td>30 Days</td>
        </tr>

        <tr class="info">
          <td class="title">Web Designing</td>
          <td class="check"><font-awesome-icon icon="fa-solid fa-check" /></td>
          <td class="check"><font-awesome-icon icon="fa-solid fa-check" /></td>
          <td class="check"><font-awesome-icon icon="fa-solid fa-check" /></td>
        </tr>

        <tr class="info">
          <td class="title">Human-Centered Design</td>
          <td class="check"><font-awesome-icon icon="fa-solid fa-check" /></td>
          <td class="check"><font-awesome-icon icon="fa-solid fa-check" /></td>
          <td class="check"><font-awesome-icon icon="fa-solid fa-check" /></td>
        </tr>

        <tr class="info">
          <td class="title">Basic Marketing</td>
          <td><font-awesome-icon icon="fa-solid fa-xmark" /></td>
          <td class="check"><font-awesome-icon icon="fa-solid fa-check" /></td>
          <td class="check"><font-awesome-icon icon="fa-solid fa-check" /></td>
        </tr>

        <tr class="info">
          <td class="title">Phyton for Everybody</td>
          <td><font-awesome-icon icon="fa-solid fa-xmark" /></td>
          <td class="check"><font-awesome-icon icon="fa-solid fa-check" /></td>
          <td class="check"><font-awesome-icon icon="fa-solid fa-check" /></td>
        </tr>

        <tr class="info">
          <td class="title">Android Developer</td>
          <td><font-awesome-icon icon="fa-solid fa-xmark" /></td>
          <td><font-awesome-icon icon="fa-solid fa-xmark" /></td>
          <td class="check"><font-awesome-icon icon="fa-solid fa-check" /></td>
        </tr>

        <tr class="info">
          <td class="title">Business English</td>
          <td><font-awesome-icon icon="fa-solid fa-xmark" /></td>
          <td><font-awesome-icon icon="fa-solid fa-xmark" /></td>
          <td class="check"><font-awesome-icon icon="fa-solid fa-check" /></td>
        </tr>

        <tr class="footer">
          <td class="none"></td>
          <td class="get">
            <div class="btn">
              <div class="button">Get It Now</div>
            </div>
          </td>
          <td class="get">
            <div class="btn">
              <div class="button">Get It Now</div>
            </div>
          </td>
          <td class="get">
            <div class="btn">
              <div class="button">Get It Now</div>
            </div>
          </td>
        </tr>

      </table>
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
  border-bottom: 1px solid #CECECE;
  padding: 80px 0;
  background-image: url('/image/background-pattern.jpg');
}

.flex {
  display: flex;
  justify-content: center;
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

table,
td {
  border: 1px solid #F2F2F2;
  border-collapse: collapse;
}

table {
  width: 100%;
  text-align: center;
  // background-color: white;

  .header>.discount {
    font-family: $font-merriweather;
    font-size: 24px;
    line-height: 36px;
    background-color: white;
    text-align: bottom;
  }

  .plan {
    background-color: #F7FDFF;
  }

  .list {
    display: flex;
    flex-direction: column;
    align-items: center;
    gap: 15px;
    padding: 25px 0;

    .name {
      font-family: $font-merriweather;
      font-size: 22px;
    }

    .price {
      font-family: 'Open Sans', sans-serif;
      font-size: 20px;
    }
  }

  .info {
    font-family: 'Open Sans', sans-serif;
    font-weight: 400;
    font-size: 20px;
    color: $text-light-gray;
    background-color: white;

    td {
      padding: 10px 0;
    }

    .title {
      font-family: $font-merriweather;
      font-size: 16px;
      text-align: left;
      padding-left: 30px;
    }

    .check {
      color: $light-blue;
    }



  }

  .footer {
    font-family: 'Open Sans', sans-serif;
    font-weight: 400;
    font-size: 20px;
    color: $text-light-gray;
  }

  .get {
    background-color: #F7FDFF;
    padding: 20px 0;

    .btn {
      display: flex;
      justify-content: center;
    }

    .button {
      width: max-content;
      font-weight: 700;
      font-size: 14px;
      text-transform: uppercase;
      line-height: 26px;
      border: 2px solid #CECECE;
      padding: 10px 25px;
      background-color: white;

      &:hover {
        background-color: $light-blue;
        color: white;
        cursor: pointer;
      }
    }
  }

}
</style>