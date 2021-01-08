<template>
  <section class="portfolio-section">
    <div class="row">
      <div class="col"></div>
      <div class="col-lg-9 col-md-11">
        <div class="row">
          <div class="col"></div>
          <div class="col-lg-5">
            <q-tabs
              v-model="tab"
              dense
              class="text-grey q-mb-lg"
              active-color="primary"
              indicator-color="secondary"
              align="justify"
              narrow-indicator
            >
              <q-tab
                v-for="(project, i) in projectsList"
                :key="i"
                :name="project.tabName"
                class="rounded-borders"
              >
                <q-img :src="require(`@/assets/${project.logo}`)" />
              </q-tab>
            </q-tabs>
          </div>
          <div class="col"></div>
        </div>

        <q-tab-panels v-model="tab" animated>
          <q-tab-panel
            v-for="(project, i) in projectsList"
            :key="i"
            :name="project.tabName"
            style="overflow-y: hidden;"
          >
            <div class="row">
              <div class="col q-pa-md">
                <div
                  class="bg-grey-1 q-pa-md shadow-10"
                  style="border-radius: 15px;"
                >
                  <q-img
                    :src="require(`@/assets/${project.desktopImg}`)"
                    style="border-radius: 15px; position: relative; z-index: 0"
                  />
                </div>
                <div
                  class="bg-grey-1 q-pa-sm shadow-10"
                  style="border-radius: 15px; width: 25%; float: right; margin-right: 75px; margin-top: -150px; z-index: 100; position: relative;"
                >
                  <q-img
                    :src="require(`@/assets/${project.mobileImg}`)"
                    style="border-radius: 15px"
                  />
                </div>
              </div>
              <div class="col q-pa-md">
                <div class="q-px-xl q-mt-lg q-mb-md">
                  <q-img
                    :src="require(`@/assets/${project.logo}`)"
                    style="width: 75px;"
                  />
                </div>
                <div
                  class="text-h4 blueballoon-font weight-700 text-grey-9 q-mb-md q-px-xl"
                >
                  {{ project.name }}
                </div>
                <div
                  class="text-body2 blueballoon-font weight-400 text-grey-7 q-mb-lg q-px-xl"
                >
                  {{ project.description }}
                </div>
                <div class="q-px-xl">
                  <q-btn
                    rounded
                    class="blueballoon-font text-bold gradient-two text-white"
                    label="Visitar"
                    no-caps
                  />
                </div>
              </div>
            </div>
          </q-tab-panel>
        </q-tab-panels>
      </div>
      <div class="col desktop-only"></div>
    </div>
  </section>
</template>

<script>
export default {
  props: ["projectsList"],
  data() {
    return {
      tab: "brewthers",
    };
  },
};
</script>
