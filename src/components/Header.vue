<template>
  <div class="container">
    <div class="top d-flex justify-content-between align-items-center">
      <div class="">Avada Health</div>

      <div>
        <ul class="d-flex list-unstyled align-items-center">
          <li>Home</li>
          <li>About</li>
          <li>Departments</li>
          <li>Articles</li>
          <li>
            <button class="btn btn-primary">Make Appointment</button>
          </li>
        </ul>
      </div>
    </div>
    <div class="center-container">
      <h2>Caring For Life</h2>
      <p>
        Lorem ipsum, dolor sit amet consectetur adipisicing elit. Perferendis
        nulla atque omnis laudantium repellendus veniam vitae quia neque
        provident accusamus ad fugit animi beatae tempore rem ut, maxime
        voluptates impedit.
      </p>
      <button class="btn btn-secondary">Learn More</button>
    </div>
  </div>
</template>

<script>
export default {
  name: "Header",
};
</script>

<style lang="scss">
@import "@/styles/header.scss";
</style>