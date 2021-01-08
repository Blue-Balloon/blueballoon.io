<template>
  <q-layout view="lHh Lpr lFf">
    <div
      class="row bg-grey-1 text-white q-pa-sm"
      style="border-bottom: solid 1px #f0f0f0"
    >
      <div class="col"></div>
      <div class="col-lg-7 col-md-8 col-xs-12">
        <div class="row">
          <q-space />
          <q-btn
            rounded
            flat
            dense
            icon="fab fa-instagram"
            color="primary"
            class="on-left"
            size="sm"
          />
          <q-btn
            rounded
            flat
            dense
            icon="fab fa-twitter"
            color="primary"
            size="sm"
          />
        </div>
      </div>
      <div class="col"></div>
    </div>
    <div class="row bg-grey-1 blueballoon-font">
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
              BlueBalloon Inc.
            </div>
          </div>
          <div class="col-lg-10 col-md-9 col-sm-9 column flex-center xs-hide">
            <ul
              class="blueballoon-navbar full-width"
              style="text-align: right"
              v-if="$route.fullPath == '/' || $route.fullPath.includes('/#')"
            >
              <li><a href="#inicio" class="weight-600">Inicio</a></li>
              <li><a href="#servicios" class="weight-600">Servicios</a></li>
              <li><a href="#nuestra-mision" class="weight-600">Nosotros</a></li>
              <li><a href="#contacto" class="weight-600">Contacto</a></li>
              <li><a href="#contacto" class="weight-600">Portafolio</a></li>
              <!-- <li style="float:right">
                <q-btn
                  rounded
                  color="white"
                  class="blueballoon-font text-bold"
                  no-caps
                >
                  <div class="text-primary">Contactanos</div>
                </q-btn>
              </li> -->
            </ul>

            <ul
              class="blueballoon-navbar full-width"
              style="text-align: right"
              v-else
            >
              <router-link to="/"
                ><i class="fas fa-arrow-left on-left" />Volver al
                inicio</router-link
              >
            </ul>
          </div>
          <q-space />
          <div
            class="col-xs-1 column flex-center lg-hide md-hide sm-hide"
            v-if="$route.fullPath == '/' || $route.fullPath.includes('/#')"
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
          <div class="col-xs-1 column flex-center mobile-only" v-else>
            <q-btn
              flat
              rounded
              dense
              class="text-primary"
              icon="fas fa-home"
              to="/"
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
        <q-btn
          fab
          icon="fab fa-whatsapp"
          color="primary"
          @click="openExternalLink('https://wa.me/50768238190')"
        />
      </q-page-sticky>
      <!-- END FLOATING ACION BTN -->
    </q-page-container>
    <q-dialog
      v-model="mobileNavDrawer"
      persistent
      maximized
      transition-show="slide-left"
      transition-hide="slide-right"
    >
      <q-card dark class="bg-primary text-white blueballoon-drawer">
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
            href="#inicio"
            @click="mobileNavDrawer = false"
            class="blueballoon-drawer-link blueballoon-font q-mb-md"
            >Inicio</a
          >
          <a
            href="#servicios"
            @click="mobileNavDrawer = false"
            class="blueballoon-drawer-link blueballoon-font text-bold q-mb-md"
            >Servicios</a
          >
          <a
            href="#nuestra-mision"
            @click="mobileNavDrawer = false"
            class="blueballoon-drawer-link blueballoon-font text-bold q-mb-md"
            >Nosotros</a
          >
          <a
            href="#contacto"
            @click="mobileNavDrawer = false"
            class="blueballoon-drawer-link blueballoon-font text-bold q-mb-md"
            >Contacto</a
          >
          <!-- <a
                        class="blueballoon-drawer-link blueballoon-font text-bold q-mb-md"
                        @click="
                            mobileNavDrawer = false
                            $router.push('/blog')
                        "
                        >Blog</a
                    > -->

          <div class="row">
            <q-space />
            <q-btn
              rounded
              flat
              dense
              icon="fab fa-facebook"
              color="primary"
              class="text-white on-left"
              size="lg"
            />
            <q-btn
              rounded
              flat
              dense
              icon="fab fa-instagram"
              color="primary"
              class="text-white on-left"
              size="lg"
            />
            <q-btn
              rounded
              flat
              dense
              icon="fab fa-twitter"
              color="primary"
              class="text-white"
              size="lg"
            />
          </div>
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
  methods: {
    openExternalLink(url) {
      window.open(url, "_blank");
    },
  },
};
</script>

<style>
@import url("https://fonts.googleapis.com/css2?family=Nunito:wght@300;400;600;700&display=swap");

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
