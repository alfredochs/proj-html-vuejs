<template>
  <div class="container">
    <div class="">
      <img src="../assets/images/icon-5.png" alt="" />
      <span>Meet Our Doctors</span>
      <p>
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Temporibus,
        esse animi? Unde cumque ad labore eaque? Exercitationem, nam? Laboriosam
        perferendis, ipsa praesentium blanditiis alias nemo labore cupiditate
        reiciendis fugit ullam!
      </p>

      <div class="d-flex justify-content-center">
        <div class="d-flex flex-column" v-for="(doctor, i) in doctors" :key="i">
          <img :src="doctor.img" alt="" />
          <h4>{{ doctor.name }}</h4>
          <span>{{ doctor.specialties }}</span>
          <p>{{ doctor.description }}</p>

          <div class="d-flex">
            <a href="#">face</a>
            <a href="#">twit</a>
            <a href="#">inst</a>
          </div>
        </div>
      </div>

      <div></div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Meet",
  data() {
    return {
      doctors: [
        {
          img: require("../assets/images/doctor-1.jpg"),
          name: "Jon Snow",
          specialties: "Anesthesiologist",
          description: "prova 1",
        },
        {
          img: require("../assets/images/doctor-2.jpg"),
          name: "Jon Snow",
          specialties: "Anesthesiologist",
          description: "prova 2",
        },
        {
          img: require("../assets/images/doctor-3.jpg"),
          name: "Jon Snow",
          specialties: "Anesthesiologist",
          description: "prova 3",
        },
      ],
    };
  },
};
</script>

<style>
</style>