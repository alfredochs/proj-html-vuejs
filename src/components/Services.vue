<template>
  <div class="container p-4">
    <div class="w-25 m-auto text-center">
      <h3>Our Health Services</h3>
      <p>
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Deserunt hic
        recusandae qui praesentium enim, iste pariatur dolore id? Id quos in
        ipsam porro fuga rem tenetur quibusdam voluptatem sint consequuntur.
      </p>
    </div>

    <div class="d-flex row">
      <div
        class="d-flex flex-column align-items-center p-4 col-4"
        v-for="(service, i) in services"
        :key="i"
      >
        <img :src="service.img" alt="" style="width: 70px" />
        <h6>{{ service.serviceType }}</h6>
        <p>{{ service.description }}</p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Services",
  data() {
    return {
      services: [
        {
          img: require("@/assets/images/icon-14.png"),
          serviceType: "REHABILITATION CENTER",
          description: "prova1",
        },
        {
          img: require("@/assets/images/icon-15.png"),
          serviceType: "DENTAL IMPLANTS",
          description: "prova2",
        },
        {
          img: require("@/assets/images/icon-16.png"),
          serviceType: "MEDICINE SEARCH",
          description: "prova3",
        },
        {
          img: require("@/assets/images/icon-11.png"),
          serviceType: "BLOOD BANK",
          description: "prova4",
        },
        {
          img: require("@/assets/images/icon-12.png"),
          serviceType: "PHARMACEUTICAL ADVICE",
          description: "prova5",
        },
        {
          img: require("@/assets/images/icon-13.png"),
          serviceType: "MEDICAL COUNSELING",
          description: "prova6",
        },
      ],
    };
  },
};
</script>

<style>
</style>