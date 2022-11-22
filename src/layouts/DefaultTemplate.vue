<template>
  <div>
    <header-component />

    <section>
      <router-view></router-view>
    </section>

    <footer-component />
  </div>
</template>

<script>
import { onBeforeMount } from "vue";
import HeaderComponent from "./components/HeaderComponent";
import FooterComponent from "./components/FooterComponent";

export default {
  name: "DefaultTemplate",
  setup() {
    onBeforeMount(() => {
      document.body.classList.add("page");
      document.body.classList.add("dark");
      document.title = "EAD com Vue.js";
    });
  },
  components: {
    HeaderComponent,
    FooterComponent,
  },
};
</script>