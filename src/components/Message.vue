<template>
  <section class="message-section">
    <div class="row xs-hide">
      <div class="col"></div>
      <div class="col-lg-7 col-md-9 col-sm-12 q-px-xl q-mb-md">
        <div class="row">
          <div class="col-lg-6 col-md-6 col-sm-6">
            <q-img
              :src="require('@/assets/innovation.webp')"
              class="rounded-borders"
            />
          </div>
          <div class="col-lg-6 col-md-6 col-sm-6 column flex-center">
            <div
              class="q-pa-xl bg-grey-1 rounded-borders shadow-2"
              style="margin-left: -100px; z-index: 0"
            >
              <div class="text-body2 text-grey-7 weight-600 blueballoon-font">
                Tecnologias modernas
              </div>
              <div class="text-h6 text-grey-9 weight-600 blueballoon-font">
                Desarrollamos utilizando tecnologias de vanguardia para mantener
                tu plataforma o sitio web siempre actualizado.
              </div>
            </div>
          </div>
        </div>
      </div>
      <div class="col"></div>
    </div>
    <div class="row xl-hide lg-hide md-hide sm-hide q-px-xl">
      <q-img
        :src="require('@/assets/innovation.webp')"
        class="rounded-borders q-mb-md"
      />
      <div class="bg-grey-1 rounded-borders shadow-2 q-pa-md">
        <div class="text-body2 text-grey-7 weight-600 blueballoon-font">
          Tecnologias modernas
        </div>
        <div class="text-h6 text-grey-9 weight-600 blueballoon-font">
          Desarrollamos utilizando tecnologias de vanguardia para mantener tu
          plataforma o sitio web siempre actualizado.
        </div>
      </div>
    </div>
  </section>
</template>
