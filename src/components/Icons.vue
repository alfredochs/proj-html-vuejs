<template>
  <div
    class="d-flex text-center w-75 m-auto"
    :class="icons.length > 4 ? 'flex-wrap' : ''"
  >
    <!-- <div class="d-flex justify-content-around m-auto text-center"> -->
    <div
      class="
        d-flex
        flex-column
        justify-content-center
        align-items-center
        intenal-padding
        small-text
      "
      :class="icons.length > 4 ? 'col-4' : ''"
      v-for="(icon, i) in icons"
      :key="i"
    >
      <img :src="icon.img" alt="" style="width: 50px" />
      <h6 class="pb-2 fw-lighter pt-2 text-uppercase">{{ icon.title }}</h6>
      <p class="xs-text fw-lighter lh-lg" style="font-size: 12px">
        {{ icon.description }}
      </p>
    </div>
  </div>
</template>

<script>
export default {
  name: "Icons",
  props: {
    icons: Array,
  },
  // methods: {
  //   maiuscole() {
  //     this.$emit("changeCase", this.icons.title);
  //   },
  // },
};
</script>

<style>
@import "../styles/icons.scss";
</style>