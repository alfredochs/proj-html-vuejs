<template>
  <div class="container-fluid my-bg-header text-white">
    <div class="container p-3">
      <div class="top d-flex justify-content-between align-items-center">
        <div>
          <img
            src="../assets/images/medical_logo_1x_light.png"
            class="w-75"
            alt=""
          />
        </div>

        <div>
          <ul
            class="
              d-flex
              list-unstyled
              align-items-center
              description-text
              small-text
            "
          >
            <li v-for="link in links" :key="link" class="pe-3">
              {{ link }}
            </li>
            <li>
              <button class="btn btn-principal small-text">
                Make Appointment
              </button>
            </li>
          </ul>
        </div>
      </div>
      <div class="m-auto col-7 padding-to-bg-img">
        <div class="w-75">
          <h1 class="fw-light">
            Caring <span class="colored-text"> For Life </span>
          </h1>
          <p class="small-text">
            Kind words can be short and easy to speak, but their echoes are
            truly endless. Avada Health fovuses on you as if was our own family.
          </p>
          <button class="btn btn-principal small-text">Learn More</button>
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
// @import "../styles/header.scss";
// .my-bg-header {
//   background-image: url("../assets/images/header-image-homepage.jpg");
//   background-size: cover;
// }
</style>