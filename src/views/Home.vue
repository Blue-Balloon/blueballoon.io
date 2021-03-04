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
            "Brewthers es un OMS (Order Management System) desarrollado exclusivamente para Brewthers Co. donde comercios como bares o restanrautes se pueden afiliar para realizar ordenes de las mejores casas cerveceras artesanales de Panama.",
          link: "https://www.brewthersco.com",
          desktopImg: "brewthers_desktop.webp",
          mobileImg: "brewthers_mobile.webp",
          tabName: "brewthers",
        },
        {
          logo: "fergarvey_logo.webp",
          name: "FerGarvey",
          description:
            "Sitio web y tienda E-commerse para el artista Fernando Garvey donde podras ver todos sus artes, empresas con las que ha trabajado, historia y comprar articulos de su marca.",
          link: "https://www.fergarvey.com",
          desktopImg: "fergarvey_desktop.webp",
          mobileImg: "fergarvey_mobile.webp",
          tabName: "fergarvey",
        },
        {
          logo: "menudigital_logo.webp",
          name: "Menu Digital",
          description:
            "Menu Digital es una solucion en linea para todos aquellos emprendedores que se dedican a la venta de consumibles, donde podran presentar su menu y recibir pedidos automaticos directo en su numero de Whatsapp, Correo o condensados en una hoja de calculo para mejor orden y contabilidad.",
          link: "https://www.mimenudigital.app",
          desktopImg: "menudigital_desktop.webp",
          mobileImg: "menudigital_mobile.webp",
          tabName: "menudigital",
        },
        {
          logo: "ygo_logo.svg",
          name: "Y-Go",
          description:
            "Plataforma automatizada para la gestion de clientes y paquetes provenientes de compras por internet, con funcionalidades como pagos en linea y sistema de lealtad.",
          link: "https://y-go.com.pa",
          desktopImg: "ygo_desktop.webp",
          mobileImg: "ygo_mobile.webp",
          tabName: "ygo",
        },
        {
          logo: "my-grades-logo.webp",
          name: "MyGrades",
          description:
            "MyGrades es un Progressive Web App (PWA) instalable en dispositivos Android y iOS con la idea de ayudar a los estudiantes universitarios a llevar sus calificaciones con calculos automaticos en base a las divisiones porcentuales de cada rubro por asignatura.",
          link: "https://grades-app.netlify.app",
          desktopImg: "my-grades-desktop.webp",
          mobileImg: "my-grades-mobile.webp",
          tabName: "mygrades",
        },
        {
          logo: "adcn_logo.webp",
          name: "Adicon Panama",
          description:
            "Sitio web desarrollado para Adicon Panama, quienes se dedican a administrar y gestionar condiminios en Panama, desde mantenimientos de los equipos en la propiedad horizontal, hasta la gestion de los recursos financieros y legales.",
          link: "https://www.adiconpanama.com",
          desktopImg: "adcn_desktop.webp",
          mobileImg: "adcn_mobile.webp",
          tabName: "ygo1",
        },
      ],
      clientsCaptions: [
        // {
        //   project: "Brewthers | Gerente Comercial",
        //   client: "Francesco Mosca",
        //   caption:
        //     "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Praesent eget orci ac orci aliquet semper. Maecenas turpis dui, iaculis quis aliquam eu, convallis ut dui. Donec eu ligula eu nulla facilisis porttitor id ac enim.",
        //   avatar: "brewthers_caption_avatar.webp",
        //   tabName: "brewthers",
        // },
        {
          project: "FerGarvey | Artista",
          client: "Fernando Garvey",
          caption:
            "Los artistas somos quisquillosos con todo lo que hacemos, incluyendo nuestra web. Ellos estan llenos de paciencia y buenas ideas.",
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
