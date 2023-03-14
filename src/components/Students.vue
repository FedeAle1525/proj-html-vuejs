<script>
export default {

}
</script>


<template>
  <section>
    <div class="container-small">
      <div class="avatar">
        <img src="/image/instructor-img-6-150x150.jpg">
      </div>

      <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Non magnam minus dolor sequi et,
        aut perferendis velit repellendus! Asperiores eveniet sunt quo nulla quisquam. Voluptatem qui itaque
        aspernatur aperiam laudantium.
      </p>

      <span class="name">Joan Collins</span>

      <span class="role">Student</span>
    </div>
  </section>
</template>


<style lang="scss" scoped>
//1 - Importo Font Google
@import url('https://fonts.googleapis.com/css2?family=Merriweather:wght@700&display=swap');
//2 - Creo Variabile con Font importato
$font-merriweather: 'Merriweather', serif;

section {
  padding: 80px 0;
  color: white;
  font-family: 'Open sans', sans-serif;
  background-image: url('/image/h5-parallax-img-1.png');
  background-position: center;
}

.container-small {
  max-width: 800px;
  margin: 0 auto;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  gap: 10px;

  .avatar {
    width: 100px;
    aspect-ratio: 1/1;
    border-radius: 50px;
    overflow: hidden;
    margin-bottom: 20px;
  }

  p {
    font-size: 18px;
    line-height: 30px;
    text-align: center;
    margin-bottom: 20px;
  }

  .name {
    font-family: $font-merriweather;
    font-size: 22px;
  }

  .role {
    font-size: 14px;
    font-weight: 700;
    text-transform: uppercase;
  }
}
</style>