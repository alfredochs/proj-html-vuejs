<template>
  <div class="bg-color-grey padding-general">
    <div class="w-75 m-auto">
      <div class="m-auto text-center my-container">
        <img src="../assets/images/icon-5.png" alt="" />
        <h2 class="fw-lighter text-uppercase">Meet our Doctors</h2>
        <div class="big-border-bottom w-50"></div>
        <p class="small-text lh-lg">
          Sed ut perpiciatis unde onmis iste natus error sit voluptatem
          accusantium doloremque laudantium, totam rem aperiam, eaque ipsa quae
          ab illo inventore varitatis et quasi architecto beatae
        </p>
      </div>

      <div class="d-flex justify-content-center gap-3 pt-3">
        <div
          class="d-flex flex-column bg-light w-25"
          v-for="(doctor, i) in doctors"
          :key="i"
        >
          <img :src="doctor.img" alt="" />
          <div class="p-3">
            <span class="doctor-name text-uppercase">{{ doctor.name }}</span>
            <br />
            <span class="pb-3 doctor-name">{{ doctor.specialties }}</span>
            <p class="card-text py-3">{{ doctor.description }}</p>
            <Social :icone="socialLogo"></Social>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import Social from "./Social.vue";
export default {
  components: { Social },
  name: "Meet",
  data() {
    return {
      doctors: [
        {
          img: require("../assets/images/doctor-1.jpg"),
          name: "JON SNOW",
          specialties: "Anesthesiologist",
          description:
            "At bero eos at accusamus et iuusto odio digissimos ducimus qui bvlanditiis praesentium voluptatum deleniti atuqe",
        },
        {
          img: require("../assets/images/doctor-2.jpg"),
          name: "TONY STARK",
          specialties: "Cardiologist",
          description:
            "At bero eos at accusamus et iuusto odio digissimos ducimus qui bvlanditiis praesentium voluptatum deleniti atuqe",
        },
        {
          img: require("../assets/images/doctor-3.jpg"),
          name: "ANNA SMITH",
          specialties: "Nurse Practitioner",
          description:
            "At bero eos at accusamus et iuusto odio digissimos ducimus qui bvlanditiis praesentium voluptatum deleniti atuqe",
        },
      ],
      socialLogo: [
        {
          title: "fa-facebook",
          bg: "face-bg",
        },
        {
          title: `fa-twitter`,
          bg: "twitter-bg",
        },
        {
          title: `fa-instagram`,
          bg: "instagram-bg",
        },
      ],
    };
  },
};
</script>

<style lang="scss">
@import "@/styles/meet.scss";
</style>