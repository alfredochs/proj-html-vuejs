<template>
  <div class="container row">
    <div class="col-4 d-flex flex-column">
      <img
        src="../assets/images/medical_logo_2x_dark.png"
        class="w-50"
        alt=""
        style=""
      />
      <p>
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Facere rerum
        atque tempora rem, illum corrupti quo obcaecati quidem quae est debitis
        doloribus laborum enim quasi aliquam exercitationem, ullam tenetur nemo?
      </p>
      <span>Learn More About Us</span>
      <div class="d-flex">
        <a href="#">face</a>
        <a href="#">twitter</a>
        <a href="#">youtube</a>
        <a href="#">instagram</a>
      </div>
    </div>
    <div class="col-4">
      <span>Contact Information</span>
      <ul class="list-unstyled">
        <li class="d-flex">
          <img
            src="../assets/images/medical_logo_2x_dark.png"
            alt=""
            width="20px"
          />
          <span>Indirizzo</span>
        </li>
        <li>Telefono</li>
      </ul>
    </div>
    <div class="col-4">
      <h6>Medical Departments</h6>
      <ul class="d-flex flex-column list-unstyled">
        <li v-for="reparto in reparti" :key="reparto">
          {{ reparto }}
        </li>
      </ul>
      <button class="col-6 btn btn-danger">View Our Departments</button>
    </div>
  </div>
</template>

<script>
export default {
  name: "Footer",
  data() {
    return {
      reparti: [
        "Cardiology",
        "Pedriatrics",
        "Diabetes Care",
        "Pren-Natel Care",
        "Ultrasound Echocardiogram",
      ],
      // [
      //   {
      //     tipo: "Cardiology",
      //   },
      //   {
      //     tipo: "Pediatrics",
      //   },
      //   {
      //     tipo: "Diabetes Care",
      //   },
      //   {
      //     tipo: "Pren-Natel Care",
      //   },
      //   {
      //     tipo: "Ultrasound Echocardiogram",
      //   },
      // ],
    };
  },
};
</script>

<style>
</style>