<template>
  <div class="main-container">
    <!-- Navbar section -->
    <HeaderShowcase />

    <!-- Intro -->
    <HeroAppShowcase />

    <!-- 1. Presentacion -->
    <Presentacion />

    <!-- 2. Cartas de presentación -->
    <Cartas />

    <!-- 3.	UC Davis EE. UU. -->
    <UCDavisUS />

    <!-- 4. three step process -->
    <RelacionHistorica />

    <!-- 5. UC Davis Chile -->
    <UCDavisChile />

    <!-- 6. Nuestra Mision -->
    <NuestraMision />

    <!-- 7. Impacto -->
    <div
      class="feature-app-showcase section-space--pt_120 section-space--mb_120 section-space--pb_120 bg-gray"
      id="impacto"
    >
      <div class="container">
        <div class="row">
          <div class="col">
            <ChartCircleTwo
              color="poppy"
              sectionProgress="63"
              circleValue="07"
              class="section-space--mb_40"
            />
          </div>
        </div>
        <SectionTitle
          color="poppy"
          sectionTitle="Impacto"
          class="wow move-up"
        />
      </div>
    </div>

    <!-- 8. Quienes somos -->
    <QuienesSomos />

    <!-- 9. Areas de trabajo -->
    <AreasTrabajo />

    <!-- 10. Proyectos -->

    <Proyectos />
    <!-- overlay menu section -->
    <OverlayMenu />

    <FooterMain />
  </div>
</template>

<script>
import HeaderShowcase from "@/components/HeaderShowcase";
import Cartas from "@/components/sections/Cartas";
import HeroAppShowcase from "@/components/HeroAppShowcase";
import UCDavisUS from "@/components/sections/UCDavisUS";
import UCDavisChile from "@/components/sections/UCDavisChile";
import Presentacion from "@/components/sections/Presentacion";
import RelacionHistorica from "@/components/sections/RelacionHistorica";
import AppShowcaseNewsletter from "@/components/sections/AppShowcaseNewsletter";
import FooterAppShowcase from "@/components/FooterAppShowcase";
import OverlayMenu from "@/components/OverlayMenu";
import SectionTitle from "@/components/SectionTitle";
import ChartCircleTwo from "@/components/ChartCircleTwo";
import NuestraMision from "@/components/sections/NuestraMision";
import QuienesSomos from "@/components/sections/QuienesSomos";
import AreasTrabajo from "@/components/sections/AreasTrabajo.vue";
import Proyectos from "@/components/sections/Proyectos.vue";
import FooterMain from "@/components/FooterMain";
export default {
  name: "app",
  components: {
    HeaderShowcase,
    Cartas,
    Cartas,
    UCDavisUS,
    HeroAppShowcase,
    Presentacion,
    RelacionHistorica,
    AppShowcaseNewsletter,
    FooterAppShowcase,
    OverlayMenu,
    ChartCircleTwo,
    SectionTitle,
    QuienesSomos,
    NuestraMision,
    AreasTrabajo,
    Proyectos,
    FooterMain,
    UCDavisChile,
  },
};
</script>

