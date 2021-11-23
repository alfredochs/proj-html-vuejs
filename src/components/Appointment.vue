<template>
  <div class="bg-appointment text-white">
    <div class="appointment-container text-center">
      <h2>Make an Appointment</h2>
      <p>
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Consectetur
        error non nisi incidunt provident ipsam doloremque cupiditate sunt
        beatae accusamus dolore eaque, officia pariatur quia impedit id
        aspernatur ipsa enim.
      </p>
    </div>

    <div class="appointment-container">
      <!-- nome e cognome -->
      <div class="row">
        <div class="mb-3 col-6">
          <label for="exampleFormControlInput1" class="form-label">Nome</label>
          <input
            type="email"
            class="form-control"
            id="exampleFormControlInput1"
            placeholder="Inserisci il tuo nome"
          />
        </div>

        <div class="mb-3 col-6">
          <label for="exampleFormControlInput1" class="form-label"
            >Email address</label
          >
          <input
            type="email"
            class="form-control"
            id="exampleFormControlInput1"
            placeholder="name@example.com"
          />
        </div>
        <div class="mb-3 col-6">
          <label for="exampleFormControlInput1" class="form-label"
            >Phone Number</label
          >
          <input
            type="email"
            class="form-control"
            id="exampleFormControlInput1"
            placeholder="Inserisci il tuo telefono"
          />
        </div>
        <div class="mb-3 col-6">
          <label for="exampleFormControlInput1" class="form-label"
            >Appointment Date</label
          >
          <input
            type="email"
            class="form-control"
            id="exampleFormControlInput1"
            placeholder="Scegli la data"
          />
        </div>
      </div>

      <!-- fine nome e cognome -->
      <!-- text area -->
      <div class="">
        <label for="exampleFormControlTextarea1" class="form-label"
          >Example textarea
        </label>
        <textarea
          class="form-control"
          id="exampleFormControlTextarea1"
          rows="3"
        ></textarea>
        <!-- text area -->
        <button class="btn btn-primary w-100 mt-2">Make an Appointment</button>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Appointment",
};
</script>

<style lang="scss">
.appointment-container {
  width: 50%;
  margin: auto;
  text-align: left;
}
.bg-appointment {
  background-image: url("../assets/images/make-an-appointment.jpg");
  background-size: cover;
}
</style>