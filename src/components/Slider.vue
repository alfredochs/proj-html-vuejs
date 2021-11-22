<template>
  <div class="container-fluid bg-danger">
    <div v-for="(image, i) in images" :key="i" style="widht: 70px"></div>
    <img :src="image.img" alt="" />
  </div>
</template>

<script>
export default {
  name: "Slider",
  dat() {
    return {
      images: [
        {
          img: require("@/assets/images/client-logos-1.png"),
        },
        {
          img: require("@/assets/images/client-logos-2.png"),
        },
        {
          img: require("@/assets/images/client-logos-3.png"),
        },
        {
          img: require("@/assets/images/client-logos-4.png"),
        },
      ],
    };
  },
};
</script>

<style>
</style>