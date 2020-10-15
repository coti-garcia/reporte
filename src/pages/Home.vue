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

    <!-- 5. newsletter section -->
    <AppShowcaseNewsletter />
    <div
      class="feature-app-showcase section-space--pt_120 section-space--mb_120 section-space--pb_120 bg-gray"
      id="mision"
    >
      <div class="container">
        <div class="row">
          <div class="col">
            <ChartCircleTwo circleValue="06" class="section-space--mb_40" />
          </div>
        </div>
        <SectionTitle sectionTitle="Nuestra misión" class="wow move-up" />
        <!-- tab conetent section -->
        <TabOne />
      </div>
    </div>
    <div
      class="feature-app-showcase section-space--pt_120 section-space--mb_120 section-space--pb_120"
      id="impacto"
    >
      <div class="container">
        <div class="row">
          <div class="col">
            <ChartCircleTwo circleValue="07" class="section-space--mb_40" />
          </div>
        </div>
        <SectionTitle sectionTitle="Impacto" class="wow move-up" />
      </div>
    </div>
    <!-- footer section -->
    <FooterAppShowcase />

    <!-- overlay menu section -->
    <OverlayMenu />
  </div>
</template>

<script>
import HeaderShowcase from "@/components/HeaderShowcase";
import Cartas from "@/components/Cartas";
import HeroAppShowcase from "@/components/HeroAppShowcase";
import UCDavisUS from "@/components/UCDavisUS";
import Presentacion from "@/components/Presentacion";
import RelacionHistorica from "@/components/RelacionHistorica";
import AppShowcaseNewsletter from "@/components/sections/AppShowcaseNewsletter";
import FooterAppShowcase from "@/components/FooterAppShowcase";
import OverlayMenu from "@/components/OverlayMenu";
import SectionTitle from "@/components/SectionTitle";
import ChartCircleTwo from "@/components/ChartCircleTwo";
import TabOne from "../components/TabOne";
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
    TabOne,
  },
};
</script>

