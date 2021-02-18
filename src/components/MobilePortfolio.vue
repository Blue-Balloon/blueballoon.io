<template>
  <div class="q-px-xl">
    <div class="q-gutter-md">
      <q-carousel
        v-model="slide"
        transition-prev="scale"
        transition-next="scale"
        swipeable
        animated
        control-color="primary"
        padding
        height="400px"
        class="rounded-borders"
        autoplay
        infinite
      >
        <q-carousel-slide
          :name="project.tabName"
          style="padding: 0 !important"
          v-for="(project, i) in formattedProjectsList"
          :key="i"
        >
          <div v-if="i % 2 == 0" class="q-pt-xl">
            <div class="bg-grey-1 shadow-2 q-pa-sm" style="border-radius: 10px">
              <q-img
                :src="require(`@/assets/${project.desktopImg}`)"
                style="border-radius: 10px; position: relative; z-index: 0"
              />
            </div>
            <div
              class="bg-grey-1 shadow-2 q-pa-xs"
              style="
                border-radius: 10px;
                width: 100px;
                margin-top: -100px;
                z-index: 100;
                position: relative;
                right: -60%;
              "
            >
              <q-img
                :src="require(`@/assets/${project.mobileImg}`)"
                style="border-radius: 10px"
              />
            </div>
          </div>
          <div v-else>
            <q-img
              :src="require(`@/assets/${project.logo}`)"
              class="q-mb-md q-mt-xl"
              style="width: 75px"
            />
            <div
              class="text-h6 blueballoon-font weight-700 text-grey-9 q-mb-sm"
            >
              {{ project.name }}
            </div>
            <div
              class="text-body2 blueballoon-font weight-600 text-grey-7 q-mb-md"
            >
              {{ project.description }}
            </div>
            <a
              :href="project.link"
              class="external-link"
              target="_blank"
              rel="noopener"
            >
              <q-btn
                label="Visitar"
                no-caps
                rounded
                class="blueballoon-font text-bold text-white gradient-two"
              />
            </a>
          </div>
        </q-carousel-slide>
      </q-carousel>
    </div>
  </div>
</template>

<script>
export default {
  props: ["projectsList"],
  data() {
    return {
      slide: "brewthers",
      formattedProjectsList: this.formatProjectsList(),
    };
  },
  methods: {
    formatProjectsList() {
      let newList = [];
      this.projectsList.forEach((project) => {
        newList.push({
          desktopImg: project.desktopImg,
          mobileImg: project.mobileImg,
          tabName: project.tabName,
        });
        newList.push({
          logo: project.logo,
          name: project.name,
          description: project.description,
          link: project.link,
          tabName: `${project.tabName}_d`,
        });
      });
      return newList;
    },
  },
};
</script>
