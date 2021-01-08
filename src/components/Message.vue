<template>
  <section class="message-section">
    <div class="row desktop-only">
      <div class="col desktop-only"></div>
      <div class="col-lg-7 q-pa-md">
        <div class="row">
          <div class="col">
            <q-img
              :src="require('@/assets/img1.jpg')"
              class="rounded-borders"
            />
          </div>
          <div class="col column flex-center">
            <div
              class="q-pa-xl bg-grey-1 rounded-borders shadow-2"
              style="margin-left: -100px; z-index: 0;"
            >
              <div class="text-body2 text-grey-7 weight-600 blueballoon-font">
                Purpose meets Enterprise
              </div>
              <div class="text-h6 text-grey-9 weight-600 blueballoon-font">
                Lorem ipsum dolor sit amet, consectetur adipiscing elit.
                Curabitur pellentesque neque eget diam posuere porta.
              </div>
            </div>
          </div>
        </div>
      </div>
      <div class="col desktop-only"></div>
    </div>
    <div class="row q-pa-md mobile-only">
      <q-img
        :src="require('@/assets/img1.jpg')"
        class="rounded-borders q-mb-md"
      />
      <div class="q-pa-md bg-grey-1 rounded-borders shadow-2 full-width">
        <div class="text-body2 text-grey-7 weight-600 blueballoon-font">
          Purpose meets Enterprise
        </div>
        <div class="text-h6 text-grey-9 weight-600 blueballoon-font">
          Lorem ipsum dolor sit amet, consectetur adipiscing elit. Curabitur
          pellentesque neque eget diam posuere porta.
        </div>
      </div>
    </div>
  </section>
</template>
