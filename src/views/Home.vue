<!-- RIP REVOSOFT -->
<template>
  <q-page>
    <Hero id="home" />
    <Services id="services" />
    <Message id="us" />
    <Gradient />
    <DesktopPortfolio
      class="xs-hide"
      :projectsList="projects"
      id="portfolio-d"
    />
    <MobilePortfolio
      class="xl-hide lg-hide md-hide sm-hide"
      :projectsList="projects"
      id="portfolio-m"
    />
    <Captions :captionsList="clientsCaptions" />
    <Contact id="contact" />
    <Footer />
  </q-page>
</template>

<script>
import Hero from "@/components/Hero";
import Services from "@/components/Services";
import Message from "@/components/Message";
import Gradient from "@/components/Gradient";
import DesktopPortfolio from "@/components/DesktopPortfolio";
import MobilePortfolio from "@/components/MobilePortfolio";
import Captions from "@/components/Captions";
import Contact from "@/components/Contact";
import Footer from "@/components/Footer";

export default {
  data() {
    return {
      projects: [
        {
          logo: "brewthers_logo.webp",
          name: "Brewthers",
          description:
            "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum diam dolor, interdum in sollicitudin lobortis, pretium vel enim. Aliquam erat volutpat. In eget ante in nisl blandit iaculis. Duis metus libero, tincidunt quis velit vel, viverra iaculis tortor.",
          link: "https://www.brewthersco.com",
          desktopImg: "brewthers_desktop.png",
          mobileImg: "brewthers_mobile.png",
          tabName: "brewthers",
        },
        {
          logo: "fergarvey_logo.png",
          name: "FerGarvey",
          description:
            "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum diam dolor, interdum in sollicitudin lobortis, pretium vel enim. Aliquam erat volutpat. In eget ante in nisl blandit iaculis. Duis metus libero, tincidunt quis velit vel, viverra iaculis tortor.",
          link: "https://www.fergarvey.com",
          desktopImg: "fergarvey_desktop.png",
          mobileImg: "fergarvey_mobile.png",
          tabName: "fergarvey",
        },
        {
          logo: "menudigital_logo.png",
          name: "Menu Digital",
          description:
            "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum diam dolor, interdum in sollicitudin lobortis, pretium vel enim. Aliquam erat volutpat. In eget ante in nisl blandit iaculis. Duis metus libero, tincidunt quis velit vel, viverra iaculis tortor.",
          link: "https://www.mimenudigital.app",
          desktopImg: "menudigital_desktop.png",
          mobileImg: "menudigital_mobile.png",
          tabName: "menudigital",
        },
        {
          logo: "ygo_logo.svg",
          name: "Y-Go",
          description:
            "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum diam dolor, interdum in sollicitudin lobortis, pretium vel enim. Aliquam erat volutpat. In eget ante in nisl blandit iaculis. Duis metus libero, tincidunt quis velit vel, viverra iaculis tortor.",
          link: "https://y-go.com.pa",
          desktopImg: "ygo_desktop.png",
          mobileImg: "ygo_mobile.png",
          tabName: "ygo",
        },
        {
          logo: "adcn_logo.webp",
          name: "Adicon Panama",
          description:
            "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum diam dolor, interdum in sollicitudin lobortis, pretium vel enim. Aliquam erat volutpat. In eget ante in nisl blandit iaculis. Duis metus libero, tincidunt quis velit vel, viverra iaculis tortor.",
          link: "https://www.adiconpanama.com",
          desktopImg: "adcn_desktop.png",
          mobileImg: "adcn_mobile.png",
          tabName: "ygo1",
        },
      ],
      clientsCaptions: [
        {
          project: "Brewthers | Gerente Comercial",
          client: "Francesco Mosca",
          caption:
            "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Praesent eget orci ac orci aliquet semper. Maecenas turpis dui, iaculis quis aliquam eu, convallis ut dui. Donec eu ligula eu nulla facilisis porttitor id ac enim.",
          avatar: "brewthers_caption_avatar.webp",
          tabName: "brewthers",
        },
        {
          project: "FerGarvey | Artista",
          client: "Fernando Garvey",
          caption:
            "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Praesent eget orci ac orci aliquet semper. Maecenas turpis dui, iaculis quis aliquam eu, convallis ut dui. Donec eu ligula eu nulla facilisis porttitor id ac enim.",
          avatar: "fergarvey_caption_avatar.webp",
          tabName: "fergarvey",
        },
      ],
    };
  },
  components: {
    Hero,
    Services,
    Message,
    Gradient,
    DesktopPortfolio,
    MobilePortfolio,
    Captions,
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

/* width */
::-webkit-scrollbar {
  width: 5px;
}

/* Track */
::-webkit-scrollbar-track {
  background-color: #fff;
}

/* Handle */
::-webkit-scrollbar-thumb {
  background: rgb(67, 192, 246) !important;
  background: linear-gradient(
    45deg,
    rgba(67, 192, 246, 1) 0%,
    rgba(92, 69, 173, 1) 100%
  ) !important;
}
</style>
