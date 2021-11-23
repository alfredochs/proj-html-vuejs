<template>
  <div id="app">
    <Header></Header>
    <Welcome></Welcome>
    <Meet></Meet>
    <Services></Services>
    <Facilities></Facilities>
    <Appointment></Appointment>
    <Slider></Slider>
    <Footer></Footer>
  </div>
</template>

<script>
import Header from "@/components/Header.vue";
import Welcome from "@/components/Welcome.vue";
import Meet from "./components/Meet.vue";
import Services from "./components/Services.vue";
import Facilities from "./components/Facilities.vue";
import Appointment from "./components/Appointment.vue";
import Slider from "./components/Slider.vue";
import Footer from "./components/Footer.vue";

export default {
  name: "App",
  components: {
    Header,
    Welcome,
    Meet,
    Services,
    Facilities,
    Appointment,
    Slider,
    Footer,
  },
};
</script>

<style lang="scss">
@import "~bootstrap/scss/bootstrap";
@import "@/styles/allStyles.scss";
@import "~font-awesome/css/font-awesome.min.css";
body {
  font-family: Arial, Helvetica, sans-serif;
}
</style>
