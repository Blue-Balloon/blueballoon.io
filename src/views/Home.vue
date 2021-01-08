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
                Vestibulum diam dolor, interdum in sollicitudin lobortis,
                pretium vel enim. Aliquam erat volutpat. In eget ante in nisl
                blandit iaculis. Duis metus libero, tincidunt quis velit vel,
                viverra iaculis tortor.
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
    <section class="contact-section bg-grey-1">
      <div class="row">
        <div class="col desktop-only"></div>
        <div class="col-lg-7">
          <div class="row q-px-md">
            <div class="text-h4 blueballoon-font weight-600 text-grey-9">
              Escribenos:
            </div>
          </div>
          <div class="row">
            <div class="col q-pa-md">
              <q-input
                label="Nombre"
                rounded
                standout="bg-primary text-white"
                class="blueballoon-font"
              />
            </div>
            <div class="col q-pa-md">
              <q-input
                label="Telefono"
                rounded
                standout="bg-primary text-white"
                class="blueballoon-font"
              />
            </div>
          </div>
          <div class="row">
            <div class="col q-pa-md">
              <q-input
                label="Correo"
                rounded
                standout="bg-primary text-white"
                class="blueballoon-font"
              />
            </div>
          </div>
          <div class="row">
            <div class="col q-pa-md">
              <q-input
                label="Mensaje"
                type="textarea"
                rows="7"
                rounded
                standout="bg-primary text-white"
                class="blueballoon-font"
              />
            </div>
          </div>
          <div class="row q-px-md">
            <q-space />
            <q-btn
              rounded
              class="blueballoon-font text-bold gradient-two text-white"
              label="Enviar"
              no-caps
            />
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
.contact-section {
  padding: 40px 0;
}
</style>
