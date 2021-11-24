<template>
  <div class="d-flex gap-2">
    <div
      v-for="(icon, i) in icone"
      :key="i"
      class="container-logo text-white p-2"
      :class="icon.bg"
    >
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