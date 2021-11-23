<template>
  <div class="d-flex">
    <div v-for="(icon, i) in icone" :key="i" class="container-logo">
      <i aria-hidden="true" class="fa" :class="icon.title"></i>
    </div>
  </div>
</template>

<script>
export default {
  name: "Social",
  props: {
    icone: Array,
  },
};
</script>

<style>
</style>