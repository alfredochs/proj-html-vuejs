<template>
  <div>
    <div class="container m-auto row padding-general">
      <div class="col-4 d-flex flex-column small-text">
        <img
          src="../assets/images/medical_logo_2x_dark.png"
          class="w-50"
          alt=""
          style=""
        />
        <p class="pt-3">
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Facere rerum
          atque tempora rem, illum corrupti quo obcaecati quidem quae est
          debitis doloribus laborum enim quasi aliquam exercitationem, ullam
          tenetur nemo?
        </p>
        <div class="full-border-top">
          <span class="fw-normal">Learn More About Us</span>
        </div>

        <Social :icone="socialLogo"></Social>
      </div>
      <div class="col-4">
        <h6 class="text-uppercase">Contact Information</h6>
        <div class="small-border-bottom"></div>
        <ul class="list-unstyled">
          <li class="d-flex gap-1">
            <i
              class="fa fa-map-marker"
              aria-hidden="true"
              style="color: #39abbb"
            ></i>

            <h6 class="small-text">121 King Street, London United Kingdom</h6>
          </li>
          <li class="d-flex gap-1">
            <i
              class="fa fa-phone"
              aria-hidden="true"
              style="color: #39abbb"
            ></i>
            <h6 class="small-text">1.800.458.556</h6>
          </li>
        </ul>
      </div>
      <div class="col-4">
        <h6 class="text-uppercase">Medical Departments</h6>
        <div class="small-border-bottom"></div>
        <ul class="d-flex flex-column list-unstyled">
          <li v-for="reparto in reparti" :key="reparto" class="small-text p-1">
            <div class="d-flex gap-2">
              <div class="reparti-footer-container p-2">
                <i
                  class="fa fa-chevron-right"
                  aria-hidden="true"
                  style="font-size: 10px"
                ></i>
              </div>
              {{ reparto }}
            </div>
          </li>
        </ul>
        <button
          class="
            btn
            fw-light
            border
            rounded-0
            button-facilities-card
            text-uppercase
          "
        >
          View Our Departments
        </button>
      </div>
    </div>
    <div class="container-fluid bg-color-grey">
      <div
        class="
          container
          d-flex
          justify-content-between
          align-items-center
          copyright-container
        "
      >
        <div class="small-text">
          Copyright 2021-2020 | Avada Theme by Theme Fusion | All Rights
          Reserved | Powered by WordPress
        </div>
        <div class="arrow-container">
          <i class="fa fa-angle-up" aria-hidden="true"></i>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import Social from "./Social.vue";
export default {
  components: { Social },
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
          title: `fa-youtube-play`,
          bg: "youtube-bg",
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
@import "@/styles/footer.scss";
</style>