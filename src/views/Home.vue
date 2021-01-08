<template>
  <q-page>
    <Hero />
    <Services />
    <Message />
    <Gradient />
    <DesktopPortfolio />
    <Contact />
    <Footer />
  </q-page>
</template>

<script>
import Hero from "@/components/Hero";
import Services from "@/components/Services";
import Message from "@/components/Message";
import Gradient from "@/components/Gradient";
import DesktopPortfolio from "@/components/DesktopPortfolio";
import Contact from "@/components/Contact";
import Footer from "@/components/Footer";

export default {
  components: {
    Hero,
    Services,
    Message,
    Gradient,
    DesktopPortfolio,
    Contact,
    Footer,
  },
};
</script>

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
  background: rgb(67, 192, 246) !important;
  background: linear-gradient(
    45deg,
    rgba(67, 192, 246, 1) 0%,
    rgba(92, 69, 173, 1) 100%
  ) !important;
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
