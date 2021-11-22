<template>
  <div class="container my-container">
    <h2>Welcome to Avada Health</h2>
    <p>
      Lorem ipsum dolor, sit amet consectetur adipisicing elit. Quidem quos
      molestiae nisi, hic possimus labore veritatis tenetur fugiat sapiente quas
      enim mollitia similique, non odio distinctio officiis laboriosam eum
      aperiam.
    </p>
    <div class="d-flex justify-content-around">
      <div
        class="d-flex flex-column justify-content-center"
        v-for="(chiave, i) in welcomeIcons"
        :key="i"
      >
        <img :src="chiave.img" alt="" class="w-50" />
        <span> {{ chiave.title }}</span>
        <span>{{ chiave.description }}</span>
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
          description: "Testo di prova 1",
          img: require("../assets/images/icon-1.png"),
        },
        {
          title: "World Class Facilities",
          description: "Testo di prova 2",
          img: require("../assets/images/icon-2.png"),
        },
        {
          title: "Experts Doctors",
          description: "Testo di prova 3",
          img: require("../assets/images/icon-3.png"),
        },
        {
          title: "Complementary Therapies",
          description: "Testo di prova 4",
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
</style>