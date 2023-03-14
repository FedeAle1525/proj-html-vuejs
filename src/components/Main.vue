<script>
import Types from './Types.vue';
import Tutoring from './Tutoring.vue';
import Children from './Children.vue';
import Students from './Students.vue';
import Info from './Info.vue';
import Courses from './Courses.vue';

export default {

  components: {
    Types,
    Tutoring,
    Children,
    Students,
    Info,
    Courses
  }
}
</script>

<template>
  <Types />

  <Tutoring />

  <Children />

  <Students />

  <Info />

  <Courses />
</template>

<style lang="scss" scoped></style>