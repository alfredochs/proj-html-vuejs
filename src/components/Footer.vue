<template>
  <div>
    <div class="container m-auto row padding-general">
      <div class="col-4 d-flex flex-column">
        <img
          src="../assets/images/medical_logo_2x_dark.png"
          class="w-50"
          alt=""
          style=""
        />
        <p>
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Facere rerum
          atque tempora rem, illum corrupti quo obcaecati quidem quae est
          debitis doloribus laborum enim quasi aliquam exercitationem, ullam
          tenetur nemo?
        </p>
        <span>Learn More About Us</span>
        <Social :icone="socialLogo"></Social>
      </div>
      <div class="col-4">
        <span>Contact Information</span>
        <ul class="list-unstyled">
          <li class="d-flex gap-1">
            <i
              class="fa fa-map-marker"
              aria-hidden="true"
              style="color: #39abbb"
            ></i>

            <h6>Indirizzo</h6>
          </li>
          <li class="d-flex gap-1">
            <i class="fa fa-phone" aria-hidden="true"></i>
            <h6>Telefono</h6>
          </li>
        </ul>
      </div>
      <div class="col-4">
        <h6>Medical Departments</h6>
        <ul class="d-flex flex-column list-unstyled">
          <li v-for="reparto in reparti" :key="reparto">
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
        <button class="btn btn-principal">View Our Departments</button>
      </div>
    </div>
    <div class="container-fluid bg-grey">
      <div class="container d-flex justify-content-between">
        <div>
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
          title: `fa-twitter-square`,
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
.reparti-footer-container {
  width: 20px;
  height: 20px;
  background-color: #39abbb;
  color: white;
  border-radius: 50%;
  display: flex;
  justify-content: center;
  align-items: center;
}
.arrow-container {
  height: 30px;
  width: 40px;
  border-top-left-radius: 20%;
  border-top-right-radius: 20%;
  background-color: #3d4954;
  color: white;
  display: flex;
  justify-content: center;
  align-items: center;
}
</style>