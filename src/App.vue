<template>
  <div id="app">
    <Header></Header>
    <Welcome></Welcome>
  </div>
</template>

<script>
import Header from "@/components/Header.vue";
import Welcome from "@/components/Welcome.vue";
export default {
  name: "App",
  components: { Header, Welcome },
};
</script>

<style lang="scss">
@import "~bootstrap/scss/bootstrap";
@import "@/styles/allStyles.scss";
</style>
