<template>
  <section class="section bg-secondary">
    <div class="container">
      <div class="row row-grid align-items-center">
        <div class="col-md-6">
          <div class="card bg-default shadow border-0">
            <img
              v-lazy="'img/theme/Screenshot 2022-04-04 193946.jpg'"
              class="card-img-top"
            />
            <blockquote class="card-blockquote">
              <svg
                preserveAspectRatio="none"
                xmlns="http://www.w3.org/2000/svg"
                viewBox="0 0 583 95"
                class="svg-bg"
              >
                <polygon
                  points="0,52 583,95 0,95"
                  class="fill-default"
                ></polygon>
                <polygon
                  points="0,42 583,95 683,0 0,95"
                  opacity=".2"
                  class="fill-default"
                ></polygon>
              </svg>
              <h4 class="display-3 font-weight-bold text-white">IMS</h4>
              <h6 class="text-success text-uppercase">Vue js</h6>
              <div>
                <badge type="success" style="color: white" rounded
                  >Vuetify</badge
                >
                <badge type="success" style="color: white" rounded
                  >Bootstrap-Vue</badge
                >
                <badge type="success" style="color: white" rounded
                  >Ag-Grid</badge
                >
              </div>
            </blockquote>
          </div>
        </div>
        <div class="col-md-6">
          <div class="pl-md-5">
            <!-- <icon
              name="ni ni-settings"
              class="mb-5"
              size="lg"
              type="warning"
              shadow
              rounded
            ></icon> -->

            <h3>IMS (Influencer Management System)</h3>
            <p>Roles based routing</p>
            <p>Awesome Grid view using ag-grid</p>
            <p>Validations using v-validator</p>
            <a
              href="http://manage.ims.directory/"
              class="font-weight-bold text-warning mt-5"
              >Go through IMS</a
            >
          </div>
        </div>
      </div>
    </div>
  </section>
</template>


<script>
export default {
  name: "projects",
  components: {},
};
</script>
