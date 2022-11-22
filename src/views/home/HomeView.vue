<template>
  <div>
    <section>
      <div class="pageTitle">
        <span class="title">Meus Cursos</span>
        <span class="dots">
          <span></span>
          <span></span>
          <span></span>
        </span>
      </div>

      <div class="content">
        <ul class="listCourses">
          <card-course
          :title="'Curso de Laravel com Vue.js 3'"
          :image="''"
          :bgName="'laravel'">
          </card-course>
        </ul>
      </div>
    </section>
  </div>
</template>

<script>
import CardCourse from "./components/CardCourse.vue";
export default {
  name: "HomeView",
  components: {
    CardCourse,
  },
};
</script>
