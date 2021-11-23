<template>
  <div class="bg-color general-padding">
    <div class="w-75 m-auto">
      <div class="w-50 m-auto text-center">
        <img src="../assets/images/icon-5.png" alt="" />
        <h2>MEET OUR DOCTORS</h2>
        <p>
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Temporibus,
          esse animi? Unde cumque ad labore eaque? Exercitationem, nam?
          Laboriosam perferendis, ipsa praesentium blanditiis alias nemo labore
          cupiditate reiciendis fugit ullam!
        </p>
      </div>

      <div class="d-flex justify-content-center gap-3">
        <div
          class="d-flex flex-column bg-light w-25"
          v-for="(doctor, i) in doctors"
          :key="i"
        >
          <img :src="doctor.img" alt="" />
          <div class="p-5">
            <h4>{{ doctor.name }}</h4>
            <span class="pb-3">{{ doctor.specialties }}</span>
            <p>{{ doctor.description }}</p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  components: {},
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
    };
  },
};
</script>

<style lang="scss">
@import "@/styles/variables.scss";
</style>