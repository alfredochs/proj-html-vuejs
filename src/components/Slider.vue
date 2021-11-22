<template>
  <div class="container-fluid bg-dark d-flex justify-content-center">
    <div v-for="(logo, i) in logos" :key="i">
      <img :src="logo.img" alt="" />
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

<style>
</style>