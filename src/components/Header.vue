<template>
  <div class="container-fluid my-bg-header text-white h-100">
    <div class="container p-3">
      <div class="top d-flex justify-content-between align-items-center">
        <div class="">
          <img
            src="../assets/images/medical_logo_1x_light.png"
            class="w-75"
            alt=""
          />
        </div>

        <div>
          <ul class="d-flex list-unstyled align-items-center description-text">
            <li v-for="link in links" :key="link" class="pe-3">
              {{ link }}
            </li>
            <li>
              <button class="btn btn-principal">Make Appointment</button>
            </li>
          </ul>
        </div>
      </div>
      <div class="center-container col-6">
        <div class="w-75">
          <h2>Caring <span class="colored-text"> For Life </span></h2>
          <p class="description-text">
            Kind words can be short and easy to speak, but their echoes are
            truly endless. Avada Health fovuses on you as if was our own family.
          </p>
          <button class="btn btn-principal">Learn More</button>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Header",
  data() {
    return {
      links: ["Home", "About", "Departments", "Articles"],
    };
  },
};
</script>

<style lang="scss">
// @import "@/styles/header.scss";
.my-bg-header {
  background-image: url("../assets/images/header-image-homepage.jpg");
  background-size: cover;
  .colored-text {
    color: #39afbb;
  }
  .btn-principal {
    background-color: #3aafbf;
    color: white;
  }
  .description-text {
    font-size: 14px;
  }
}
</style>