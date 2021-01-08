<template>
  <q-page>
    <section class="hero-section bg-grey-1">
      <div class="row">
        <div class="col desktop-only"></div>
        <div class="col-lg-7 q-pa-md">
          <div class="row">
            <div class="col">
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
            <div class="col">
              <q-img :src="require('@/assets/macbook.svg')" />
            </div>
          </div>
        </div>
        <div class="col desktop-only"></div>
      </div>
    </section>
    <section class="services-section">
      <div class="row">
        <div class="col desktop-only"></div>
        <div class="col-lg-7">
          <div class="row">
            <div class="col-lg-4 q-pa-md">
              <div class="service-icon gradient-one q-mb-md">
                <span class="material-icons">
                  color_lens
                </span>
              </div>
              <div
                class="text-h6 blueballoon-font weight-600 text-grey-9 q-mb-md"
              >
                Awesome design
              </div>
              <div
                class="text-body2 blueballoon-font weight-300 text-grey-7 q-mb-lg"
              >
                Purpose is a great free UI package based on Bootstrap 4 that
                includes the most important components and features.
              </div>
            </div>
            <div class="col-lg-4 q-pa-md">
              <div class="service-icon gradient-two q-mb-md">
                <span class="material-icons">
                  code
                </span>
              </div>
              <div
                class="text-h6 blueballoon-font weight-600 text-grey-9 q-mb-md"
              >
                Intuitive code
              </div>
              <div
                class="text-body2 blueballoon-font weight-300 text-grey-7 q-mb-lg"
              >
                Purpose is a great free UI package based on Bootstrap 4 that
                includes the most important components and features.
              </div>
            </div>
            <div class="col-lg-4 q-pa-md">
              <div class="service-icon gradient-three q-mb-md">
                <span class="material-icons">
                  settings
                </span>
              </div>
              <div
                class="text-h6 blueballoon-font weight-600 text-grey-9 q-mb-md"
              >
                Helpful build tools
              </div>
              <div
                class="text-body2 blueballoon-font weight-300 text-grey-7 q-mb-lg"
              >
                Purpose is a great free UI package based on Bootstrap 4 that
                includes the most important components and features.
              </div>
            </div>
          </div>
        </div>
        <div class="col desktop-only"></div>
      </div>
    </section>
    <section class="message-section">
      <div class="row">
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
    </section>
    <section class="gradient-section ">
      <div class="row">
        <div class="col desktop-only"></div>
        <div class="col-lg-7 q-pa-md">
          <div style="width: 50%; margin: 0 auto;">
            <div
              class="text-h3 blueballoon-font weight-300 text-center q-mb-lg"
            >
              See it. Love it
            </div>
            <div class="text-body2 blueballoon-font weight-300 text-center">
              A unique and beautiful collection of UI elements that are all
              flexible and modular. A complete and customizable solution to
              building the website of your dreams.
            </div>
          </div>
        </div>
        <div class="col desktop-only"></div>
      </div>
    </section>
    <section class="portfolio-section">
      <div class="row">
        <div class="col desktop-only"></div>
        <div class="col-lg-9">
          <!-- <div class="row">
            clients
          </div> -->
          <div class="row">
            <div class="col q-pa-lg">
              <div
                class="bg-grey-1 q-pa-md shadow-10"
                style="border-radius: 15px;"
              >
                <q-img
                  :src="require('@/assets/brewthers.png')"
                  style="border-radius: 15px;"
                />
              </div>
              <div
                class="bg-grey-1 q-pa-sm shadow-10"
                style="border-radius: 15px; width: 25%; float: right; margin-right: 75px; margin-top: -150px;"
              >
                <q-img
                  :src="require('@/assets/brewthers_mobile.png')"
                  style="border-radius: 15px"
                />
              </div>
            </div>
            <div class="col">2</div>
          </div>
        </div>
        <div class="col desktop-only"></div>
      </div>
    </section>
  </q-page>
</template>

<style>
.hero-section {
  padding: 75px 0;
}

.services-section {
  padding: 50px 0;
}
.service-icon {
  text-align: center;
  width: 50px;
  height: 50px;
  padding-top: 4px;
  border-radius: 25px;
  color: #fff;
  font-size: 25px;
}
.gradient-one {
  background: rgb(70, 244, 242);
  background: linear-gradient(
    45deg,
    rgba(70, 244, 242, 1) 0%,
    rgba(86, 144, 241, 1) 100%
  );
}
.gradient-two {
  background: rgb(67, 192, 246);
  background: linear-gradient(
    45deg,
    rgba(67, 192, 246, 1) 0%,
    rgba(92, 69, 173, 1) 100%
  );
}
.gradient-three {
  background: rgb(86, 144, 241);
  background: linear-gradient(
    45deg,
    rgba(86, 144, 241, 1) 0%,
    rgba(63, 49, 100, 1) 100%
  );
}
.message-section {
  padding-bottom: 40px;
}

.gradient-section {
  padding: 50px 0;
  background: rgb(67, 192, 246);
  background: linear-gradient(
    180deg,
    rgba(67, 192, 246, 1) 0%,
    rgba(86, 144, 241, 1) 100%
  );
  color: #fff;
}
.portfolio-section {
  padding: 50px 0;
}
</style>
