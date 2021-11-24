<template>
  <div class="bg-color-grey padding-general">
    <div class="w-75 m-auto">
      <div class="m-auto text-center my-container">
        <img src="../assets/images/icon-5.png" alt="" />
        <h2 class="fw-lighter">MEET OUR DOCTORS</h2>
        <div class="big-border-bottom w-50"></div>
        <p class="small-text">
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Temporibus,
          esse animi? Unde cumque ad labore eaque? Exercitationem, nam?
          Laboriosam perferendis, ipsa praesentium blanditiis alias nemo labore
          cupiditate reiciendis fugit ullam!
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
            <span class="doctor-name">{{ doctor.name }}</span> <br />
            <span class="pb-3 doctor-name">{{ doctor.specialties }}</span>
            <p class="small-text">{{ doctor.description }}</p>
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