<template>
  <div class="header">
    <div class="row">
      <div class="col hide-sm hide-xs"></div>
      <div class="col-lg-7 col-md-8 col-sm-12 q-pa-xl">
        <div class="row q-pt-xl">
          <q-space />
          <div
            class="col-lg-6 col-md-6 col-sm-6 col-xs-12 xl-hide lg-hide md-hide q-mb-md"
          >
            <q-img :src="require('@/assets/macbook.webp')" />
          </div>
          <q-space />
          <div
            class="col-lg-12 col-md-12 col-sm-12 col-xs-12 column flex-center text-center q-mb-md"
          >
            <div
              class="text-h4 blueballoon-font weight-400 text-white q-mb-md q-pr-md"
              style="
                font-size: 3rem;
                line-height: 3.5rem;
                text-transform: uppercase;
              "
            >
              Llevamos tus ideas a la realidad.
            </div>
            <div
              class="text-subtitle2 blueballoon-font weight-300 text-white q-mb-lg q-pr-md"
            >
              Te ayudamos a cumplir tus metas y sueños en una realidad tangible,
              utilizando tecnologías de vanguardia en un mundo altamente
              competitivo.
            </div>
            <div class="full-width">
              <a href="#contact" style="text-decoration: none" v-smooth-scroll>
                <q-btn
                  rounded
                  color="white"
                  push
                  class="blueballoon-font text-bold gradient-two"
                  text-color="primary"
                  label="Contáctanos"
                  no-caps
                />
              </a>
            </div>
          </div>
          <div
            class="col-lg-12 col-md-12 col-sm-12 col-xs-12 xs-hide sm-hide column flex-center"
            style="margin-bottom: -150px;"
          >
            <q-img
              :src="require('@/assets/macbook.webp')"
              style="width: 500px;"
            />
          </div>
        </div>
      </div>
      <div class="col hide-sm hide-xs"></div>
    </div>

    <!--Waves Container-->
    <div>
      <svg
        class="waves"
        xmlns="http://www.w3.org/2000/svg"
        xmlns:xlink="http://www.w3.org/1999/xlink"
        viewBox="0 24 150 28"
        preserveAspectRatio="none"
        shape-rendering="auto"
      >
        <defs>
          <path
            id="gentle-wave"
            d="M-160 44c30 0 58-18 88-18s 58 18 88 18 58-18 88-18 58 18 88 18 v44h-352z"
          />
        </defs>
        <g class="parallax">
          <use
            xlink:href="#gentle-wave"
            x="48"
            y="0"
            fill="rgba(255,255,255,0.7)"
          />
          <use
            xlink:href="#gentle-wave"
            x="48"
            y="3"
            fill="rgba(255,255,255,0.5)"
          />
          <use
            xlink:href="#gentle-wave"
            x="48"
            y="5"
            fill="rgba(255,255,255,0.3)"
          />
          <use xlink:href="#gentle-wave" x="48" y="7" fill="#fff" />
        </g>
      </svg>
    </div>
    <!--Waves end-->
  </div>
</template>

<style>
/* .header {
  position: relative;
  background-color: white;
  color: white;
} */
.trex {
  transition-timing-function: ease;
  transition-timing-function: cubic-bezier(0.25, 0.1, 0.25, 1);
  transform: translateY(150px);
  animation: popup 5s 0s ease infinite;
}
@keyframes popup {
  0% {
    transform: translateY(-15px);
  }
  50% {
    transform: translateY(15px);
  }
  100% {
    transform: translateY(-15px);
  }
}
.header {
  background: linear-gradient(270deg, #43c0f6, #5690f1);
  background-size: 400% 400%;

  -webkit-animation: AnimationName 24s ease infinite;
  -moz-animation: AnimationName 24s ease infinite;
  animation: AnimationName 24s ease infinite;
}

@-webkit-keyframes AnimationName {
  0% {
    background-position: 0% 50%;
  }
  50% {
    background-position: 100% 50%;
  }
  100% {
    background-position: 0% 50%;
  }
}
@-moz-keyframes AnimationName {
  0% {
    background-position: 0% 50%;
  }
  50% {
    background-position: 100% 50%;
  }
  100% {
    background-position: 0% 50%;
  }
}
@keyframes AnimationName {
  0% {
    background-position: 0% 50%;
  }
  50% {
    background-position: 100% 50%;
  }
  100% {
    background-position: 0% 50%;
  }
}
.waves {
  position: relative;
  width: 100%;
  height: 15vh;
  margin-bottom: -7px; /*Fix for safari gap*/
  min-height: 100px;
  max-height: 150px;
}

/* Animation */

.parallax > use {
  animation: move-forever 25s cubic-bezier(0.55, 0.5, 0.45, 0.5) infinite;
}
.parallax > use:nth-child(1) {
  animation-delay: -2s;
  animation-duration: 7s;
}
.parallax > use:nth-child(2) {
  animation-delay: -3s;
  animation-duration: 10s;
}
.parallax > use:nth-child(3) {
  animation-delay: -4s;
  animation-duration: 13s;
}
.parallax > use:nth-child(4) {
  animation-delay: -5s;
  animation-duration: 20s;
}
@keyframes move-forever {
  0% {
    transform: translate3d(90px, 0, 0);
  }
  100% {
    transform: translate3d(-85px, 0, 0);
  }
}
/*Shrinking for mobile*/
@media (max-width: 768px) {
  .waves {
    height: 40px;
    min-height: 40px;
  }
  .content {
    height: 30vh;
  }
  h1 {
    font-size: 24px;
  }
}
</style>
