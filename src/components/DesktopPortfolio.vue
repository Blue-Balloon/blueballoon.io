<template>
  <section class="portfolio-section">
    <div class="row">
      <div class="col desktop-only"></div>
      <div class="col-lg-9">
        <!-- <div class="row">
            clients
          </div> -->
        <div class="row">
          <div class="col q-pa-md">
            <div
              class="bg-grey-1 q-pa-md shadow-10"
              style="border-radius: 15px;"
            >
              <q-img
                :src="require('@/assets/brewthers.png')"
                style="border-radius: 15px; position: relative; z-index: 0"
              />
            </div>
            <div
              class="bg-grey-1 q-pa-sm shadow-10"
              style="border-radius: 15px; width: 25%; float: right; margin-right: 75px; margin-top: -150px; z-index: 100; position: relative;"
            >
              <q-img
                :src="require('@/assets/brewthers_mobile.png')"
                style="border-radius: 15px"
              />
            </div>
          </div>
          <div class="col q-pa-md">
            <div
              class="text-h4 blueballoon-font weight-700 text-grey-9 q-mt-xl q-mb-md q-px-xl"
            >
              Brewthers
            </div>
            <div
              class="text-body2 blueballoon-font weight-400 text-grey-7 q-mb-lg q-px-xl"
            >
              Lorem ipsum dolor sit amet, consectetur adipiscing elit.
              Vestibulum diam dolor, interdum in sollicitudin lobortis, pretium
              vel enim. Aliquam erat volutpat. In eget ante in nisl blandit
              iaculis. Duis metus libero, tincidunt quis velit vel, viverra
              iaculis tortor.
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
      </div>
      <div class="col desktop-only"></div>
    </div>
  </section>
</template>
