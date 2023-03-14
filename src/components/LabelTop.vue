<script>
export default {

}
</script>

<template>
  <div class="label">
    <font-awesome-icon icon="fa-solid fa-angle-up" />

    <span>top</span>
  </div>
</template>


<style lang="scss" scoped>
@use '../style/partials/variables' as *;

.label {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  width: 58px;
  aspect-ratio: 1;
  background-color: $light-blue;
  color: white;

  span {
    font-family: 'Open Sans', sans-serif;
    font-size: 13px;
    font-weight: 700;
    text-transform: uppercase;
  }

}
</style>