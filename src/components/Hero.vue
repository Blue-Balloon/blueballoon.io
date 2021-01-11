<template>
  <div class="header">
    <div class="row">
      <div class="col hide-sm hide-xs"></div>
      <div class="col-lg-7 col-md-8 col-sm-12 q-pa-md">
        <div class="row q-pt-xl">
          <div
            class="col-lg-6 col-md-6 col-sm-6 col-xs-12 xl-hide lg-hide md-hide sm-hide q-mb-md"
          >
            <q-img :src="require('@/assets/macbook.png')" />
          </div>
          <div class="col-lg-6 col-md-6 col-sm-6 col-xs-12 q-pt-xl q-mb-lg">
            <div
              class="text-h4 blueballoon-font weight-400 text-white q-mb-md"
              style="font-size: 2.4rem;"
            >
              A new era of web development.
            </div>
            <div
              class="text-body2 blueballoon-font weight-300 text-white q-mb-lg"
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
          <div
            class="col-lg-6 col-md-6 col-sm-6 col-xs-12 xs-hide column flex-center"
          >
            <q-img :src="require('@/assets/macbook.png')" />
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
            fill="rgba(255,255,255,0.7"
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
.header {
  position: relative;
  background: linear-gradient(
    45deg,
    rgba(67, 192, 246, 1) 0%,
    rgba(92, 69, 173, 1) 100%
  );
  color: white;
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
    transform: translate3d(-90px, 0, 0);
  }
  100% {
    transform: translate3d(85px, 0, 0);
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
