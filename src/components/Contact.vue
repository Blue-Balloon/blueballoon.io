<template>
  <section class="contact-section bg-grey-1">
    <div class="row">
      <div class="col desktop-only"></div>
      <div class="col-lg-7 col-md-8">
        <div class="row q-px-md">
          <div class="text-h4 blueballoon-font weight-600 text-grey-9">
            Escribenos:
          </div>
        </div>
        <div class="row">
          <div class="col-lg-6 col-md-6 col-xs-12 q-pa-md">
            <q-input
              label="Nombre"
              rounded
              standout="bg-primary text-white"
              class="blueballoon-font"
            />
          </div>
          <div class="col-lg-6 col-md-6 col-xs-12 q-pa-md">
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
</template>
