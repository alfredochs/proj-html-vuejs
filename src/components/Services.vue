<template>
  <div class="container padding-general w-75">
    <div class="my-container m-auto text-center">
      <img src="../assets/images/icon-6.png" alt="" />
      <h2 class="fw-lighter">OUR HEALTH SERVICES</h2>
      <div class="big-border-bottom"></div>

      <p class="small-text">
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Deserunt hic
        recusandae qui praesentium enim, iste pariatur dolore id? Id quos in
        ipsam porro fuga rem tenetur quibusdam voluptatem sint consequuntur.
      </p>
    </div>
    <Icons :icons="services"></Icons>
  </div>
</template>

<script>
import Icons from "./Icons.vue";
export default {
  components: { Icons },
  name: "Services",
  data() {
    return {
      services: [
        {
          img: require("@/assets/images/icon-14.png"),
          title: "REHABILITATION CENTER",
          description:
            "At vero eos et accusaus et iiusto odio dignissimos ducimusq ui nblandiotiis praesetoim voliptatum deleniti atque corrupti quos dolores et quas",
        },
        {
          img: require("@/assets/images/icon-15.png"),
          title: "DENTAL IMPLANTS",
          description:
            "At vero eos et accusaus et iiusto odio dignissimos ducimusq ui nblandiotiis praesetoim voliptatum deleniti atque corrupti quos dolores et quas",
        },
        {
          img: require("@/assets/images/icon-16.png"),
          title: "MEDICINE SEARCH",
          description:
            "At vero eos et accusaus et iiusto odio dignissimos ducimusq ui nblandiotiis praesetoim voliptatum deleniti atque corrupti quos dolores et quas",
        },
        {
          img: require("@/assets/images/icon-11.png"),
          title: "BLOOD BANK",
          description:
            "At vero eos et accusaus et iiusto odio dignissimos ducimusq ui nblandiotiis praesetoim voliptatum deleniti atque corrupti quos dolores et quas",
        },
        {
          img: require("@/assets/images/icon-12.png"),
          title: "PHARMACEUTICAL ADVICE",
          description:
            "At vero eos et accusaus et iiusto odio dignissimos ducimusq ui nblandiotiis praesetoim voliptatum deleniti atque corrupti quos dolores et quas",
        },
        {
          img: require("@/assets/images/icon-13.png"),
          title: "MEDICAL COUNSELING",
          description:
            "At vero eos et accusaus et iiusto odio dignissimos ducimusq ui nblandiotiis praesetoim voliptatum deleniti atque corrupti quos dolores et quas",
        },
      ],
    };
  },
};
</script>

<style lang="scss">
@import "@/styles/variables.scss";
</style>