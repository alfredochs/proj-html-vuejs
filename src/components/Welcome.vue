<template>
  <div class="w-75 m-auto">
    <div class="container my-container" style="max-width: 35%">
      <h3>Welcome to Avada Health</h3>
      <p class="description-text">
        Sed ut perspiciatis unde omnis iste natus error sit voluptatem
        accusantoum doloremque laudantium, totam rem aperiam, eaque ipsa quae ab
        illo.
      </p>
    </div>

    <div class="d-flex justify-content-around m-auto text-center">
      <div
        class="d-flex flex-column justify-content-center align-items-center"
        v-for="(chiave, i) in welcomeIcons"
        :key="i"
      >
        <img :src="chiave.img" alt="" class="w-25" />
        <div class="">
          <h6 class="pb-2">{{ chiave.title }}</h6>
          <span class="description-text">{{ chiave.description }}</span>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
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
};
</script>

<style lang="scss">
.my-container {
  width: 70%;
  margin: auto;
  text-align: center;
}
.description-text {
  font-size: 14px;
}
</style>