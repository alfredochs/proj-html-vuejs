<template>
  <div id="app">
    <Header></Header>
    <Welcome></Welcome>
    <Meet></Meet>
    <Services></Services>
    <!-- commenti di prova per commit -->
  </div>
</template>

<script>
import Header from "@/components/Header.vue";
import Welcome from "@/components/Welcome.vue";
import Meet from "./components/Meet.vue";
import Services from "./components/Services.vue";
export default {
  name: "App",
  components: { Header, Welcome, Meet, Services },
};
</script>

<style lang="scss">
@import "~bootstrap/scss/bootstrap";
@import "@/styles/allStyles.scss";
</style>
