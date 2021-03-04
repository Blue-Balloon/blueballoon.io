<template>
  <section>
    <div class="row q-px-md q-mb-lg">
      <div class="col"></div>
      <div class="col-lg-7 col-md-10 col-sm-11 col-xs-12">
        <div class="row">
          <div
            class="col-lg-12 q-px-lg q-mb-xl"
            v-for="(caption, i) in captionsList"
            :key="i"
          >
            <div
              class="text-h6 blueballoon-font weight-300 text-grey-7 q-mb-md"
              style="/*min-height: 150px*/"
            >
              <em> "{{ caption.caption }}" </em>
            </div>
            <q-item>
              <q-item-section side>
                <q-avatar size="60px">
                  <q-img :src="require(`@/assets/${caption.avatar}`)" />
                </q-avatar>
              </q-item-section>
              <q-item-section>
                <q-item-label>
                  <div class="text-h6 blueballoon-font weight-600 text-grey-9">
                    {{ caption.client }}
                  </div>
                </q-item-label>
                <q-item-label caption>
                  <div
                    class="text-body2 blueballoon-font weight-400 text-grey-9"
                  >
                    - {{ caption.project }}
                  </div>
                </q-item-label>
              </q-item-section>
            </q-item>
          </div>
          <!-- <q-carousel
            v-model="slide"
            transition-prev="slide-right"
            transition-next="slide-left"
            animated
            infinite
            swipeable
            autoplay
            class="q-mb-lg"
            style="height: auto !important"
          >
            <q-carousel-slide
              :name="caption.tabName"
              v-for="(caption, i) in captionsList"
              :key="i"
            >
              <div
                class="text-h6 blueballoon-font weight-300 text-grey-7 q-mb-md"
              >
                <em> "{{ caption.caption }}" </em>
              </div>
              <q-item>
                <q-item-section side>
                  <q-avatar size="60px">
                    <q-img :src="require(`@/assets/${caption.avatar}`)" />
                  </q-avatar>
                </q-item-section>
                <q-item-section>
                  <q-item-label>
                    <div
                      class="text-h6 blueballoon-font weight-600 text-grey-9"
                    >
                      {{ caption.client }}
                    </div>
                  </q-item-label>
                  <q-item-label caption>
                    <div
                      class="text-body2 blueballoon-font weight-400 text-grey-9"
                    >
                      - {{ caption.project }}
                    </div>
                  </q-item-label>
                </q-item-section>
              </q-item>
            </q-carousel-slide>
          </q-carousel> -->
        </div>
      </div>
      <div class="col"></div>
    </div>
  </section>
</template>

<script>
export default {
  props: ["captionsList"],
  data() {
    return {
      slide: "brewthers",
    };
  },
};
</script>
