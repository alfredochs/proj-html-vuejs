<template>
  <div id="app">
    <Header></Header>
    <Welcome></Welcome>
    <Meet></Meet>
  </div>
</template>

<script>
import Header from "@/components/Header.vue";
import Welcome from "@/components/Welcome.vue";
import Meet from "./components/Meet.vue";
export default {
  name: "App",
  components: { Header, Welcome, Meet },
};
</script>

<style lang="scss">
@import "~bootstrap/scss/bootstrap";
@import "@/styles/allStyles.scss";
</style>
