<template>
  <div>
    <div class="container-fluid bg-facilities" style="padding: 150px 0">
      <div class="container">
        <div
          class="
            d-flex
            flex-column
            align-items-center
            text-center
            my-container
            m-auto
            text-white
          "
        >
          <img src="../assets/images/icon-7.png" alt="" style="width: 40px" />
          <h2 class="fw-lighter text-uppercase">TO OUR FACILITIES</h2>
          <div class="big-border-bottom w-50"></div>

          <p class="small-text lh-lg">
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

    <div class="d-flex row text-center">
      <div
        class="
          d-flex
          flex-column
          col-4
          align-items-center
          text-white
          padding-cards
        "
        :class="card.bg"
        v-for="(card, i) in cards"
        :key="i"
      >
        <h5 class="fw-light small-text">{{ card.title }}</h5>
        <img :src="card.img" alt="" style="width: 50px" />
        <p class="fw-lighter p-2" style="font-size: 10px">
          {{ card.description }}
        </p>
        <button
          class="
            btn
            text-white
            border
            rounded-0
            text-uppercase
            button-facilities-card
          "
        >
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
          bg: "primo-colore",
          description:
            "Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque laudantium, totam rem aperiam, eaque",
        },
        {
          title: "Experts Diagnostics",
          img: require("@/assets/images/wave-divider.png"),
          btnText: "Learn More 2",
          bg: "secondo-colore",
          description:
            "Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque laudantium, totam rem aperiam, eaque",
        },
        {
          title: "Super Rehabilitation",
          img: require("@/assets/images/wave-divider.png"),
          btnText: "Learn More 3",
          bg: "terzo-colore",
          description:
            "Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque laudantium, totam rem aperiam, eaque",
        },
      ],
    };
  },
};
</script>

<style lang="scss">
@import "@/styles/facilities.scss";

.bg-facilities {
  background-image: url("../assets/images/paralax-bg-tour-facilities.jpg");
  background-size: cover;
  background-position: center;
}
</style>