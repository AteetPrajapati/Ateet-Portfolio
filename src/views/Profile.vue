<template>
  <div class="profile-page">
    <section class="section-profile-cover section-shaped my-0">
      <div class="shape shape-style-1 shape-primary shape-skew alpha-4">
        <span></span>
        <span></span>
        <span></span>
        <span></span>
        <span></span>
        <span></span>
        <span></span>
      </div>
    </section>
    <section
      class="section section-skew"
      style="
        background: linear-gradient(150deg, black 15%, #322a42 70%, black 94%);
      "
    >
      <div class="container">
        <card shadow class="card-profile mt--300" style="z-index: 1">
          <div class="px-4">
            <div class="row justify-content-center">
              <div class="col-lg-3 order-lg-2">
                <div class="card-profile-image">
                  <a>
                    <img
                      v-lazy="'img/theme/IMG_20220114_155926.jpg'"
                      class="rounded-circle"
                    />
                  </a>
                </div>
              </div>
              <div
                class="col-lg-4 order-lg-3 text-lg-right align-self-lg-center"
              >
                <div class="card-profile-actions py-4 mt-lg-0">
                  <base-button type="info" size="sm" class="mr-4"
                    >Connect</base-button
                  >
                  <base-button type="default" size="sm" class="float-right"
                    >Message</base-button
                  >
                </div>
              </div>
              <div class="col-lg-4 order-lg-1">
                <div class="card-profile-stats d-flex justify-content-center">
                  <div>
                    <span class="heading">1.5 </span>
                    <span class="description">Exprience Years</span>
                  </div>
                  <div>
                    <span class="heading">5</span>
                    <span class="description">Projects</span>
                  </div>
                  <!-- <div>
                    <span class="heading">89</span>
                    <span class="description">Comments</span>
                  </div> -->
                </div>
              </div>
            </div>
            <div class="text-center mt-5">
              <h3>
                Ateet Prajapati
                <span class="font-weight-light">, 20</span>
              </h3>
              <div class="h6 font-weight-300">
                <i class="ni location_pin mr-2"></i>Gujarat, India
              </div>
              <div class="h6 mt-2">
                <i class="ni business_briefcase-24 mr-2"></i>Computer Science
                End Engineerinng
              </div>
              <div>
                <i class="ni education_hat mr-2"></i>Gujarat Technological
                University
              </div>
            </div>
            <div class="p-2">
              <div class="row justify-content-center">
                <div class="col-lg-12">
                  <base-alert type="default">
                    <!-- <span class="alert-inner--icon"
                      ><i class="ni ni-like-2"></i
                    ></span> -->
                    <span class="alert-inner--text">
                      <ul>
                        <li>
                          An ambitious problem solver with a passion for remote
                          work, and who would like to join a team of minded
                          developers.
                        </li>
                        <li>
                          I have much experience of creating both logical and
                          innovative solutions to complex web problems.
                        </li>
                      </ul>
                    </span>
                  </base-alert>
                </div>
              </div>
              <div class="row">
                <div class="col-lg-12">
                  <base-button type="primary">
                    <span>Skills</span>
                    <badge type="default" style="color: white">10</badge>
                  </base-button>
                </div>
                <div class="col-lg-6 mt-4">
                  <div class="mycutom-tab">
                    <div>
                      <base-progress
                        type="danger"
                        :value="90"
                        label="html"
                      ></base-progress>
                      <base-progress
                        type="danger"
                        :value="90"
                        label="css"
                      ></base-progress>
                      <base-progress
                        type="danger"
                        :value="90"
                        label="javascript"
                      ></base-progress>
                      <base-progress
                        type="danger"
                        :value="90"
                        label="Vuejs (Vue2)"
                      ></base-progress>
                      <base-progress
                        type="danger"
                        :value="80"
                        label="Reactjs"
                      ></base-progress>
                    </div>
                  </div>
                </div>
                <div class="col-lg-6 mt-4">
                  <div class="mycutom-tab">
                    <div>
                      <base-progress
                        type="danger"
                        :value="85"
                        label="bootstrap-vue"
                      ></base-progress>
                      <base-progress
                        type="danger"
                        :value="90"
                        label="vuetify"
                      ></base-progress>
                      <base-progress
                        type="danger"
                        :value="90"
                        label="ag-grid"
                      ></base-progress>
                      <base-progress
                        type="danger"
                        :value="90"
                        label="ioniic-vue"
                      ></base-progress>
                      <base-progress
                        type="danger"
                        :value="70"
                        label="redux"
                      ></base-progress>
                    </div>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </card>
      </div>
    </section>
  </div>
</template>
<script>
import Tabs from "@/components/Tabs/Tabs";
import TabPane from "@/components/Tabs/TabPane";
export default {
  components: {
    Tabs,
    TabPane,
  },
};
</script>
<style scoped>
.progress-wrapper {
  padding-top: 0px;
}
</style>
