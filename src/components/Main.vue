<script>
import Types from './Types.vue';
import Tutoring from './Tutoring.vue';
import Children from './Children.vue';
import Students from './Students.vue';
import Info from './Info.vue';

export default {

  components: {
    Types,
    Tutoring,
    Children,
    Students,
    Info
  }
}
</script>

<template>
  <Types />

  <Tutoring />

  <Children />

  <Students />

  <Info />
</template>

<style lang="scss" scoped></style>