<script>
export default {

}
</script>


<template>
  <div class="container">

    <span>© 2017 Qode Interactive, All Rights Reserved</span>

    <ul>
      <li class="phone">Call +44 300 303 0266 </li>
      <li class="social">Follow Us</li>
      <li><font-awesome-icon icon="fa-brands fa-twitter" class="icon" /></li>
      <li><font-awesome-icon icon="fa-brands fa-instagram" class="icon" /></li>
      <li><font-awesome-icon icon="fa-brands fa-facebook-f" class="icon" /></li>
    </ul>
  </div>
</template>


<style lang="scss" scoped>
@use '../style/partials/variables' as *;

.container {
  border-top: 1px solid #959595;
  color: #959595;
  font-family: 'Open Sans', sans-serif;
  padding: 50px 0;
  display: flex;
  justify-content: space-between;

  span {
    font-size: 14px;
  }

  ul {
    display: flex;
    font-size: 12px;
    gap: 20px;

    .phone,
    .social {
      text-transform: uppercase;
    }

    .icon:hover {
      color: $light-blue;
      cursor: pointer;
    }
  }
}
</style>