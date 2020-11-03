<template>
  <div
    class="feature-app-showcase section-space--pt_120 section-space--pb_120 bg-blue"
    id="proyectos"
  >
    <div class="container">
      <div class="row">
        <div class="col">
          <ChartCircleTwo
            color="cabernet"
            sectionProgress="100"
            circleValue="10"
            class="section-space--mb_40"
          />
        </div>
      </div>
      <SectionTitle
        color="white"
        sectionTitle="Principales Proyectos"
        class="wow move-up"
      />
    </div>
    <!-- portfolio item wrapper start -->
    <div class="portfolio-pages-wrapper">
      <div class="container">
        <div
          class="row clearfix masonry-wrap"
          v-masonry
          transition-duration="3s"
          item-selector=".masonary-item"
        >
          <div
            class="col-lg-4 col-md-6 masonary-item wow move-up"
            v-for="portfolio in portfolios"
            :key="portfolio.id"
          >
            <div class="portfolio-grid-caption mb-30">
              <router-link to="/portfolio-details" class="single-grid-caption">
                <div class="single-portfolio__thumbnail">
                  <img
                    class="img-fluid"
                    :src="portfolio.image"
                    :alt="portfolio.alt"
                  />
                </div>
              </router-link>
              <div class="post-info">
                <div class="post-categories carbernet">
                  {{ portfolio.category }}
                </div>
                <h5 class="post-title font-weight--bold">
                  <router-link to="/portfolio-details">{{
                    portfolio.overlayTitle
                  }}</router-link>
                </h5>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
    <!-- portfolio item wrapper end -->

    <!-- footer section -->
  </div>
</template>

<script>
import HeaderElement from "@/components/HeaderElement";
import Breadcrumb from "@/components/Breadcrumb";
import FooterMain from "@/components/FooterMain";
import OffcanvasSearchBox from "@/components/OffcanvasSearchBox";
import OffCanvasMobileMenu from "@/components/OffCanvasMobileMenu";
import SectionTitle from "@/components/SectionTitle";
import ChartCircleTwo from "@/components/ChartCircleTwo";
export default {
  name: "PortfolioMasonry",
  components: {
    HeaderElement,
    Breadcrumb,
    FooterMain,
    OffcanvasSearchBox,
    OffCanvasMobileMenu,
    SectionTitle,
    ChartCircleTwo,
  },

  mounted() {
    if (typeof this.$redrawVueMasonry === "function") {
      this.$redrawVueMasonry();
    }

    this.onLoad();
  },

  methods: {
    async onLoad() {
      await this.sleep(950);
      this.$redrawVueMasonry();
    },
    sleep(ms) {
      return new Promise((resolve) => setTimeout(resolve, ms));
    },
  },

  data() {
    return {
      portfolios: [
        {
          id: 1,
          image: require("@/assets/img/projects/01/01.jpg"),
          alt: "proyecto image",
          overlayTitle:
            "Programa de extensión y difusión tecnológica en estructuras de conducción y protección en frutales.",
          category: "Agroinchalam",
        },
        {
          id: 2,
          image: require("@/assets/img/projects/02/01.jpg"),
          alt: "proyecto image",
          overlayTitle:
            "Daño foliar en Araucaria araucana: agente causal y medidas de mitigación",
          category: "Araucarias",
        },
        {
          id: 3,
          image: require("@/assets/img/projects/03/01.jpg"),
          alt: "proyecto image",
          overlayTitle:
            "Caracterización y optimización de bioinsumos producidos a partir de camas de producción avícola.",
          category: "Ariztía",
        },
        {
          id: 4,
          image: require("@/assets/img/projects/04/01.jpg"),
          alt: "proyecto image",
          overlayTitle:
            "Determinación de línea base para el desarrollo de biofertilizantes a partir de desechos de la producción de mitílidos.",
          category: "Cal Austral",
        },
        {
          id: 5,
          image: require("@/assets/img/projects/05/01.jpg"),
          alt: "proyecto image",
          overlayTitle: "Centro de Extensionismo Vitivinícola del Sur (CEVS)",
          category: "Centro de extensión",
        },
        {
          id: 6,
          image: require("@/assets/img/projects/06/01.jpg"),
          alt: "proyecto image",
          overlayTitle: "Chile Lagos Limpios",
          category: "(ChLL)",
        },
        {
          id: 7,
          image: require("@/assets/img/projects/07/01.jpg"),
          alt: "proyecto image",
          overlayTitle:
            "Central de información y modelación hídrica de la cuenca del río Aconcagua",
          category: "CIMHI",
        },
        {
          id: 8,
          image: require("@/assets/img/projects/08/01.jpg"),
          alt: "proyecto image",
          overlayTitle:
            "Whole genome analytics, genetic identification of clones for grapevine.",
          category: "Clones de la vid / ID Clones",
        },
        {
          id: 9,
          image: require("@/assets/img/projects/09/01.jpg"),
          alt: "proyecto image",
          overlayTitle:
            "Estudio “Economía circular en el sector agroalimentario",
          category: "Economía circular",
        },
        {
          id: 10,
          image: require("@/assets/img/projects/10/01.jpg"),
          alt: "proyecto image",
          overlayTitle: "Electric Vehicle Invention",
          category: "Endófitos",
        },
        {
          id: 11,
          image: require("@/assets/img/projects/11/01.jpg"),
          alt: "proyecto image",
          overlayTitle: "Electric Vehicle Invention",
          category: "ESPOL",
        },
        {
          id: 12,
          image: require("@/assets/img/projects/12/01.jpg"),
          alt: "proyecto image",
          overlayTitle: "Electric Vehicle Invention",
          category: "HUB OEA",
        },
        {
          id: 13,
          image: require("@/assets/img/projects/13/01.jpg"),
          alt: "proyecto image",
          overlayTitle: "Electric Vehicle Invention",
          category: "Kit Lamp",
        },
        {
          id: 14,
          image: require("@/assets/img/projects/14/01.jpg"),
          alt: "proyecto image",
          overlayTitle: "Electric Vehicle Invention",
          category: "Maleza de tomates",
        },
        {
          id: 15,
          image: require("@/assets/img/projects/15/01.jpg"),
          alt: "proyecto image",
          overlayTitle: "Electric Vehicle Invention",
          category: "Marcadores de calidad",
        },
        {
          id: 16,
          image: require("@/assets/img/projects/16/01.jpg"),
          alt: "proyecto image",
          overlayTitle: "Electric Vehicle Invention",
          category: "Infiltración de acuíferos",
        },
        {
          id: 17,
          image: require("@/assets/img/projects/17/01.jpg"),
          alt: "proyecto image",
          overlayTitle: "Electric Vehicle Invention",
          category: "Proyecto Arica",
        },
        {
          id: 18,
          image: require("@/assets/img/projects/18/01.jpg"),
          alt: "proyecto image",
          overlayTitle: "Electric Vehicle Invention",
          category: "Surface Renewal",
        },
        {
          id: 19,
          image: require("@/assets/img/projects/19/01.jpg"),
          alt: "proyecto image",
          overlayTitle: "Electric Vehicle Invention",
          category: "Telemedicina",
        },
        {
          id: 20,
          image: require("@/assets/img/projects/20/01.jpg"),
          alt: "proyecto image",
          overlayTitle: "Electric Vehicle Invention",
          category: "Plant pathogens detection",
        },
      ],
    };
  },
};
</script>

