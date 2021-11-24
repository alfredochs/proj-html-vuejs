<template>
  <div class="container-fluid bg-slider d-flex justify-content-center">
    <div v-for="(logo, i) in logos" :key="i">
      <img :src="logo.img" alt="" class="w-75" />
    </div>
  </div>
</template>

<script>
export default {
  name: "Slider",
  data() {
    return {
      logos: [
        {
          img: require("@/assets/images/client-logos-1.png"),
          prova: "prova",
        },
        {
          img: require("@/assets/images/client-logos-2.png"),
          prova: "prova",
        },
        {
          img: require("@/assets/images/client-logos-3.png"),
          prova: "prova",
        },
        {
          img: require("@/assets/images/client-logos-4.png"),
          prova: "prova",
        },
      ],
    };
  },
};
</script>

<style lang="scss">
@import "@/styles/variables.scss";

.bg-slider {
  background: rgb(52, 111, 171);
  background: linear-gradient(
    90deg,
    rgba(52, 111, 171, 1) 0%,
    rgba(81, 181, 185, 1) 52%
  );
}
</style>