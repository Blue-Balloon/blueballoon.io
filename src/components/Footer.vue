<template>
  <section>
    <div class="row gradient-two q-py-xl">
      <div class="col"></div>
      <div class="col-lg-7 col-md-9 q-pa-md">
        <div class="row q-mb-lg">
          <div class="col-lg-4 col-md-4 col-sm-12 col-xs-12">
            <div class="q-mb-md">
              <q-img :src="require('@/assets/logo.webp')" width="50px" />
            </div>

            <div
              class="text-body2 text-white blueballoon-font text-bold q-mb-sm"
            >
              BlueBalloon Inc.
            </div>
            <div
              class="text-body text-white blueballoon-font q-mb-md weight-300"
            >
              Nos encargamos de traer a la vida tus ideas y proyectos
              tecnologicos, guiandote a lo largo de todo el proceso, desde la
              idea concepto hasta concretar un producto funcional.
            </div>
          </div>
          <div class="col"></div>
          <div class="col-lg-2 col-md-2 col-sm-4 col-xs-6">
            <div class="text-body2 text-white adicon-font-2 text-bold q-mb-sm">
              Enlaces
            </div>
            <a
              class="blueballoon-font text-white q-mb-sm"
              href="#home"
              v-smooth-scroll
              style="text-decoration: none; display: block"
              >Inicio</a
            >
            <a
              class="blueballoon-font text-white q-mb-sm"
              href="#services"
              v-smooth-scroll
              style="text-decoration: none; display: block"
              >Servicios</a
            >
            <a
              class="blueballoon-font text-white q-mb-sm"
              href="#us"
              v-smooth-scroll
              style="text-decoration: none; display: block"
              >Nosotros</a
            >
            <a
              class="blueballoon-font text-white xs-hide q-mb-sm"
              href="#portfolio-d"
              v-smooth-scroll
              style="text-decoration: none; display: block"
              >Portafolio</a
            >
            <a
              class="blueballoon-font text-white xl-hide lg-hide md-hide sm-hide q-mb-sm"
              href="#portfolio-m"
              v-smooth-scroll
              style="text-decoration: none; display: block"
              >Portafolio</a
            >
            <a
              class="blueballoon-font text-white q-mb-lg"
              href="#contact"
              v-smooth-scroll
              style="text-decoration: none; display: block"
              >Contacto</a
            >
          </div>
          <div class="col-lg-2 col-md-2 col-sm-4 col-xs-6">
            <div class="text-body2 text-white adicon-font-2 text-bold q-mb-sm">
              Siguenos
            </div>
            <a
              href="https://www.instagram.com/blueballoon.io/"
              rel="noopener"
              target="_blank"
              class="blueballoon-font text-white q-mb-sm"
              style="text-decoration: none; display: block"
              ><i class="fab fa-instagram "></i>&nbsp;blueballoon.io</a
            >
            <a
              href="https://twitter.com/BlueBalloon_io"
              rel="noopener"
              target="_blank"
              class="blueballoon-font text-white q-mb-sm"
              style="text-decoration: none; display: block"
              ><i class="fab fa-twitter "></i>&nbsp;BlueBalloon_io</a
            >
          </div>
          <div class="col-lg-3">
            <div class="text-body2 text-white adicon-font-2 text-bold q-mb-sm">
              Contactanos
            </div>
            <a
              href="tel:6480-6778"
              rel="noopener"
              target="_blank"
              class="blueballoon-font text-white q-mb-sm"
              style="text-decoration: none; display: block"
              ><i class="fas fa-phone-alt "></i>&nbsp;6480-6778</a
            >
            <a
              href="mailto:contacto@blueballoon.io"
              rel="noopener"
              target="_blank"
              class="blueballoon-font text-white q-mb-sm"
              style="text-decoration: none; display: block"
              ><i class="far fa-envelope "></i>&nbsp;contacto@blueballoon.io</a
            >
          </div>
        </div>
        <div class="row">
          <q-separator color="white" class="q-mb-lg" />
          <div
            class="text-body2 blueballoon-font text-white text-center full-width"
          >
            Copyright &copy; {{ new Date().getFullYear() }} Todos los derechos
            reservados.
          </div>
        </div>
      </div>
      <div class="col"></div>
    </div>
  </section>
</template>
