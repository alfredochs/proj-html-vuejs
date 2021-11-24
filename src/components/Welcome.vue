<template>
  <div class="w-75 m-auto padding-general">
    <div class="container my-container">
      <h3 class="fw-lighter">Welcome to Avada Health</h3>
      <p class="small-text">
        Sed ut perspiciatis unde omnis iste natus error sit voluptatem
        accusantoum doloremque laudantium, totam rem aperiam, eaque ipsa quae ab
        illo.
      </p>
    </div>
    <Icons :icons="welcomeIcons"></Icons>
  </div>
</template>

<script>
import Icons from "./Icons.vue";
export default {
  components: { Icons },
  name: "Welcome",
  data() {
    return {
      welcomeIcons: [
        {
          title: "Same Day Appointments",
          description:
            "Sed ut perspiciatis unde omnis iste natus error sit voluptam accusantim",
          img: require("../assets/images/icon-1.png"),
        },
        {
          title: "World Class Facilities",
          description:
            "Sed ut perspiciatis unde omnis iste natus error sit voluptam accusantim",
          img: require("../assets/images/icon-2.png"),
        },
        {
          title: "Experts Doctors",
          description:
            "Sed ut perspiciatis unde omnis iste natus error sit voluptam accusantim",
          img: require("../assets/images/icon-3.png"),
        },
        {
          title: "Complementary Therapies",
          description:
            "Sed ut perspiciatis unde omnis iste natus error sit voluptam accusantim",
          img: require("../assets/images/icon-4.png"),
        },
      ],
    };
  },
  methods: {
    maiuscole() {
      const titolo = this.welcomeIcons.title;
      console.log(titolo);
    },
  },
};
</script>

<style lang="scss">
@import "@/styles/welcome.scss";
</style>