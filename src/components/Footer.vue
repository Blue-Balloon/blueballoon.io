<template>
  <section>
    <div class="row gradient-two q-py-xl">
      <div class="col desktop-only"></div>
      <div class="col-lg-7 q-pa-md">
        <div class="row q-mb-lg">
          <div class="col-lg-4 col-md-4 col-xs-12">
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
              Nos caracterizamos por la seriedad y responsabilidad, presentando
              siempre una gran disponibilidad para atender a nuestros clientes.
            </div>
          </div>
          <div class="col"></div>
          <div class="col-lg-2 col-md-2 col-xs-6">
            <div
              class="text-body2 text-white blueballoon-font text-bold q-mb-sm"
            >
              Enlaces
            </div>
            <a
              class="blueballoon-font text-white q-mb-sm"
              style="text-decoration: none; display: block"
              >Inicio</a
            >
            <a
              class="blueballoon-font text-white q-mb-sm"
              style="text-decoration: none; display: block"
              >Servicios</a
            >
            <a
              class="blueballoon-font text-white q-mb-sm"
              style="text-decoration: none; display: block"
              >Nosotros</a
            >
            <a
              class="blueballoon-font text-white q-mb-sm"
              style="text-decoration: none; display: block"
              >Contacto</a
            >
          </div>
          <div class="col-lg-2 col-md-2 col-xs-6">
            <div class="text-body2 text-white adicon-font-2 text-bold q-mb-sm">
              Siguenos
            </div>
            <a
              href="https://www.instagram.com/adiconpanama/"
              target="_blank"
              class="blueballoon-font text-white q-mb-sm"
              style="text-decoration: none; display: block"
              ><i class="fab fa-instagram "></i>&nbsp;adiconpanama</a
            >
            <a
              href="https://twitter.com/AdiconP"
              target="_blank"
              class="blueballoon-font text-white q-mb-sm"
              style="text-decoration: none; display: block"
              ><i class="fab fa-twitter "></i>&nbsp;adiconP</a
            >
            <a
              href="https://www.facebook.com/adicon.panama.3"
              target="_blank"
              class="blueballoon-font text-white q-mb-sm"
              style="text-decoration: none; display: block"
              ><i class="fab fa-facebook "></i>&nbsp;adiconpanama</a
            >
          </div>
          <div class="col-lg-3">
            <div
              class="text-body2 text-white blueballoon-font text-bold q-mb-sm"
            >
              Contactanos
            </div>
            <a
              href="tel:6823-8190"
              target="_blank"
              class="blueballoon-font text-white q-mb-sm"
              style="text-decoration: none; display: block"
              ><i class="fas fa-phone-alt "></i>&nbsp;6823-8190</a
            >
            <a
              href="mailto:info@adiconpanama.com"
              target="_blank"
              class="blueballoon-font text-white q-mb-sm"
              style="text-decoration: none; display: block"
              ><i class="far fa-envelope "></i>&nbsp;info@adiconpanama.com</a
            >
            <a
              href="https://goo.gl/maps/XFsL7dPTCAyPPVir8"
              target="_blank"
              class="blueballoon-font text-white q-mb-sm"
              style="text-decoration: none; display: block"
              ><i class="fas fa-map-marker-alt"></i>&nbsp;Panamá, Ancón, Edif.
              Altamira Gardens Torre E #405</a
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
      <div class="col desktop-only"></div>
    </div>
  </section>
</template>
