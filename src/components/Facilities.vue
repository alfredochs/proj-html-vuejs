<template>
  <div>
    <div class="container-fluid p-5 bg-facilities" style="padding: 150px 0">
      <div class="container">
        <div
          class="
            d-flex
            flex-column
            align-items-center
            text-center
            w-50
            m-auto
            text-white
          "
        >
          <img src="../assets/images/icon-7.png" alt="" style="width: 40px" />
          <h4>To our Facilities</h4>
          <p>
            Lorem, ipsum dolor sit amet consectetur adipisicing elit. Fuga
            consectetur, expedita quisquam ut, id nam numquam eveniet sunt vel
            minus harum voluptas fugiat est dicta eos ipsum cupiditate sint
            officiis?
          </p>
          <img
            src="../assets/images/play-icon.png"
            alt=""
            style="width: 40px"
          />
        </div>
      </div>
    </div>

    <div class="d-flex row bg-danger text-center">
      <div
        class="d-flex flex-column col-4 align-items-center my-bg"
        v-for="(card, i) in cards"
        :key="i"
      >
        <h5>{{ card.title }}</h5>
        <img :src="card.img" alt="" style="width: 50px" />
        <p>{{ card.description }}</p>
        <button class="btn">
          {{ card.btnText }}
        </button>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Facilities",
  data() {
    return {
      cards: [
        {
          title: "Emergency Care",
          img: require("@/assets/images/wave-divider.png"),
          btnText: "Learn More 1",
        },
        {
          title: "Experts Diagnostics",
          img: require("@/assets/images/wave-divider.png"),
          btnText: "Learn More 2",
        },
        {
          title: "Super Rehabilitation",
          img: require("@/assets/images/wave-divider.png"),
          btnText: "Learn More 3",
        },
      ],
    };
  },
};
</script>

<style lang="scss">
.bg-facilities {
  background-image: url("../assets/images/paralax-bg-tour-facilities.jpg");
  background-size: cover;
}
</style>