<template>
  <section class="hero-section bg-grey-1">
    <div class="row">
      <div class="col desktop-only"></div>
      <div class="col-lg-7 q-pa-md">
        <div class="row">
          <div class="col-lg-6 col-md-6 col-xs-12">
            <div
              class="text-h4 blueballoon-font weight-400 text-grey-9 q-mb-md"
            >
              A new era of web development.
            </div>
            <div
              class="text-body2 blueballoon-font weight-300 text-grey-7 q-mb-lg"
            >
              Build responsive, mobile-first projects on the web with the
              world's most popular front-end component library.
            </div>
            <q-btn
              rounded
              class="blueballoon-font text-bold gradient-two text-white"
              label="Get started"
              no-caps
            />
          </div>
          <div class="col-lg-6 col-md-6 col-xs-12">
            <q-img :src="require('@/assets/macbook.svg')" />
          </div>
        </div>
      </div>
      <div class="col desktop-only"></div>
    </div>
  </section>
</template>
