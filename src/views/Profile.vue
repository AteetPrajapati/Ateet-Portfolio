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
    <section class="section section-skew">
      <div class="container">
        <card shadow class="card-profile mt--300" no-body>
          <div class="px-4">
            <div class="row justify-content-center">
              <div class="col-lg-3 order-lg-2">
                <div class="card-profile-image">
                  <a href="#">
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
              <div class="h6 mt-4">
                <i class="ni business_briefcase-24 mr-2"></i>Computer Science
                End Engineerinng
              </div>
              <div>
                <i class="ni education_hat mr-2"></i>Gujarat Technological
                University
              </div>
            </div>
            <div class="mt-5 py-5 border-top">
              <div class="row justify-content-center">
                <div class="col-lg-9">
                  <base-alert type="primary">
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
                <div class="col-lg-6">
                  <div class="mycutom-tab">
                    <tabs>
                      <tab-pane>
                        <span slot="title" class="nav-link-icon d-block"
                          >Vue Teachnology</span
                        >

                        <div>
                          <base-progress
                            type="default"
                            :value="60"
                            label="Task completed"
                          ></base-progress>
                          <base-progress
                            type="primary"
                            :value="60"
                            label="Task completed"
                          ></base-progress>
                        </div>
                      </tab-pane>
                      <tab-pane>
                        <span slot="title" class="nav-link-icon d-block"
                          >React js</span
                        >
                      </tab-pane>
                    </tabs>
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
<style>
</style>
