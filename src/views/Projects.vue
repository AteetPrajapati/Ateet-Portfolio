<template>
  <section class="section bg-secondary">
    <div class="container">
      <div class="row row-grid align-items-center">
        <div class="col-md-6">
          <div class="card bg-default shadow border-0">
            <img :src="item.img" class="card-img-top" />
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
              <h4 class="display-3 font-weight-bold text-white">
                {{ item.name }}
              </h4>
              <h6 class="text-success text-uppercase">{{ item.framework }}</h6>
              <div>
                <badge
                  v-for="(plug, i) in item.design_framework"
                  :key="i"
                  type="success"
                  style="color: white"
                  rounded
                  >{{ plug }}</badge
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

            <h3>{{ item.full_name }}</h3>
            <ul>
              <li v-for="(point, i) in item.points" :key="i">
                <p>
                  {{ point }}
                </p>
              </li>
            </ul>
            <a
              :href="item.url"
              target="blank"
              class="font-weight-bold text-warning mt-5"
              >Go through {{ item.name }}</a
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
  data() {
    return {
      items: [
        {
          id: 1,
          name: "IMS",
          framework: "Vue js",
          img: "img/theme/Screenshot 2022-04-04 193946.jpg",
          design_framework: ["vuetify", "bootstrap-vue", "ag-grid"],
          url: "http://manage.ims.directory/",
          full_name: "IMS (Influencer Management System)",
          points: [
            "Roles based routing.",
            "Awesome Grid view using ag-grid.",
            "Validations using v-validator.",
            "Single Component used for every ads creation.",
          ],
        },
        {
          id: 2,
          name: "CPX Dashboard",
          img: "img/theme/Screenshot 2022-04-04 194613.jpg",
          framework: "Vue js (Vue-2)",
          design_framework: ["vuetify", "bootstrap-vue", "Sweetalert2"],
          url: "https://dash.cpxaffiliate.com/#/dashboard",
          full_name: "CPX (Affiliate)",
          points: [
            "Particular Affiliate registar & login.",
            "Awesome Grid view using ag-grid with side filter options.",
            "Infinite Scrolling.",
            "Pagination from Server Side in Tables.",
          ],
        },
        {
          id: 3,
          name: "TABO",
          img: "img/theme/Screenshot 2022-04-04 194940.jpg",
          framework: "React js ",
          design_framework: [
            "reactstrap",
            "QR-code-generator",
            "responsive-table",
          ],
          url: "https://dev.tabo.io",
          full_name: "Travel. Access. Book. Organize",
          points: [
            "Different-different forms on selected resturant,beach,bar,pool.",
            "Menu Uploader and generate QR Code of uploaded menu.",
            "Responsive table which change th list view and card view corresponding your device.",
            "Supported i18n with two langauges ( English, Romanian).",
          ],
        },
      ],
    };
  },
  computed: {
    item() {
      console.log(this.$router.currentRoute.params.id);
      return this.items.find(
        (e) => e.id == this.$router.currentRoute.params.id
      );
    },
  },
};
</script>
