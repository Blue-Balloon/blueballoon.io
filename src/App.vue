<template>
  <q-layout view="lHh Lpr lFf">
    <!-- <div
      class="row bg-grey-1 text-white q-pa-sm"
      style="border-bottom: solid 1px #f0f0f0"
    >
      <div class="col"></div>
      <div class="col-lg-7 col-md-8 col-xs-12">
        <div class="row">
          <q-space />
          <a
            href="https://www.instagram.com/blueballoon.io/"
            class="external-link"
            target="_blank"
            rel="noopener"
          >
            <q-btn
              rounded
              flat
              dense
              icon="fab fa-instagram"
              color="primary"
              class="on-left"
              size="sm"
            >
              <span class="hidden">Instagram</span>
            </q-btn>
          </a>
          <a
            href="https://twitter.com/BlueBalloon_io"
            class="external-link"
            target="_blank"
            rel="noopener"
          >
            <q-btn
              rounded
              flat
              dense
              icon="fab fa-twitter"
              color="primary"
              size="sm"
            />
          </a>
        </div>
      </div>
      <div class="col"></div>
    </div> -->
    <div class="row bg-grey-1 blueballoon-font sticky-header shadow-5">
      <div class="col"></div>
      <div class="col-lg-7 col-md-9 col-sm-12 col-xs-12">
        <div class="row q-pa-md">
          <div class="col-lg-2 col-md-3 col-sm-3 col-xs-7">
            <q-img
              :src="require('@/assets/logo_2.webp')"
              width="20px"
              style="display: inline-block"
            />
            <div
              class="text-body text-dark blueballoon-font weight-700 on-right"
              style="display: inline-block"
            >
              Blue Balloon Inc.
            </div>
          </div>
          <div class="col-lg-10 col-md-9 col-sm-9 column flex-center xs-hide">
            <ul class="blueballoon-navbar full-width" style="text-align: right">
              <li>
                <a href="#home" v-smooth-scroll class="weight-600">Inicio</a>
              </li>
              <li>
                <a href="#services" v-smooth-scroll class="weight-600"
                  >Servicios</a
                >
              </li>
              <!-- <li>
                <a href="#us" v-smooth-scroll class="weight-600">Nosotros</a>
              </li> -->
              <li>
                <a href="#portfolio-d" v-smooth-scroll class="weight-600"
                  >Portafolio</a
                >
              </li>
              <li>
                <a href="#contact" v-smooth-scroll class="weight-600"
                  >Contacto</a
                >
              </li>
            </ul>
          </div>
          <q-space />
          <div
            class="col-xs-1 column flex-center xl-hide lg-hide md-hide sm-hide"
          >
            <q-btn
              flat
              rounded
              dense
              class="text-primary"
              icon="fas fa-bars"
              @click="mobileNavDrawer = true"
            />
          </div>
        </div>
      </div>
      <div class="col"></div>
    </div>
    <q-page-container>
      <router-view />
      <!-- FLOATING ACTION BTN -->
      <q-page-sticky position="bottom-right" :offset="[18, 18]">
        <a
          href="https://wa.me/50764806778"
          class="external-link"
          target="_blank"
          rel="noopener"
        >
          <q-btn fab icon="fab fa-whatsapp" color="primary" name="Whatsapp" />
        </a>
      </q-page-sticky>
      <!-- END FLOATING ACION BTN -->
    </q-page-container>
    <q-dialog
      v-model="mobileNavDrawer"
      persistent
      maximized
      transition-show="flip-right"
      transition-hide="flip-left"
    >
      <q-card dark class="gradient-two text-white blueballoon-drawer">
        <q-card-section>
          <div class="row">
            <q-space />
            <q-btn
              flat
              round
              icon="fas fa-times"
              @click="mobileNavDrawer = false"
            />
          </div>
        </q-card-section>
        <q-card-section>
          <a
            href="#home"
            @click="mobileNavDrawer = false"
            class="blueballoon-drawer-link blueballoon-font text-bold q-mb-md"
            >Inicio</a
          >
          <a
            href="#services"
            @click="mobileNavDrawer = false"
            class="blueballoon-drawer-link blueballoon-font text-bold q-mb-md"
            >Servicios</a
          >
          <!-- <a
            href="#us"
            @click="mobileNavDrawer = false"
            class="blueballoon-drawer-link blueballoon-font text-bold q-mb-md"
            >Nosotros</a
          > -->
          <a
            href="#portfolio-m"
            @click="mobileNavDrawer = false"
            class="blueballoon-drawer-link blueballoon-font text-bold q-mb-md"
            >Portafolio</a
          >
          <a
            href="#contact"
            @click="mobileNavDrawer = false"
            class="blueballoon-drawer-link blueballoon-font text-bold q-mb-md"
            >Contacto</a
          >
          <!-- <div class="row">
            <q-space />
            <a
              href="https://www.instagram.com/blueballoon.io/"
              class="external-link"
              target="_blank"
            >
              <q-btn
                rounded
                flat
                dense
                icon="fab fa-instagram"
                color="primary"
                class="text-white on-left"
                size="lg"
              />
            </a>
            <a
              href="https://twitter.com/BlueBalloon_io"
              class="external-link"
              target="_blank"
            >
              <q-btn
                rounded
                flat
                dense
                icon="fab fa-twitter"
                color="primary"
                class="text-white"
                size="lg"
              />
            </a>
          </div> -->
        </q-card-section>
      </q-card>
    </q-dialog>
  </q-layout>
</template>

<script>
export default {
  data() {
    return {
      mobileNavDrawer: false,
    };
  },
};
</script>

<style>
.blueballoon-font {
  font-family: "Nunito", sans-serif;
}
.weight-300 {
  font-weight: 300 !important;
}
.weight-400 {
  font-weight: 400 !important;
}
.weight-600 {
  font-weight: 600 !important;
}
.weight-700 {
  font-weight: 700 !important;
}
.external-link {
  text-decoration: none;
}
.sticky-header {
  position: -webkit-sticky !important;
  position: sticky !important;
  top: 0 !important;
  z-index: 1000;
}
.blueballoon-navbar {
  text-align: left;
  margin: 0;
}
.blueballoon-navbar li {
  display: inline-block;
  margin-left: 45px;
}
.blueballoon-navbar a {
  text-decoration: none;
  font-size: 14px;
  color: #5690f1;
}

.blueballoon-drawer a {
  display: block;
  color: #fff;
  text-decoration: none;
  font-size: 35px;
  text-align: right;
}
</style>
