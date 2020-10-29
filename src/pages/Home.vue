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
    <div class="container-fluid section-space--ptb_120 bg-gray">
      <div class="row">
        <div class="col-lg-12">
          <ChartCircleTwo
            circleValue="05"
            class="section-space--mb_40 section-space--mt_30"
            color="icing"
            sectionProgress="50"
          />
          <SectionTitle
            color="icing"
            sectionTitle="UC Davis Chile"
            class="wow move-up"
          />
        </div>
      </div>
    </div>

    <NuestraMision />
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
    <!-- footer section -->
    <QuienesSomos />
    <div
      class="feature-app-showcase section-space--pt_120 section-space--mb_120 section-space--pb_120 bg-gray"
      id="areas-trabajo"
    >
      <div class="container">
        <div class="row">
          <div class="col">
            <ChartCircleTwo
              color="bodega"
              sectionProgress="81"
              circleValue="09"
              class="section-space--mb_40"
            />
          </div>
        </div>
        <SectionTitle
          color="bodega"
          sectionTitle="Áreas de trabajo UC Davis Chile"
          class="wow move-up"
        />
      </div>
    </div>
    <div
      class="feature-app-showcase section-space--pt_120 section-space--mb_120 section-space--pb_120"
      id="alianzas"
    >
      <div class="container">
        <div class="row">
          <div class="col">
            <ChartCircleTwo
              color="cabernet"
              sectionProgress="90"
              circleValue="10"
              class="section-space--mb_40"
            />
          </div>
        </div>
        <SectionTitle
          color="cabernet"
          sectionTitle="Principales alianzas"
          class="wow move-up"
        />
      </div>
    </div>
    <div
      class="feature-app-showcase section-space--mb_120 section-space--pb_120"
      id="proyectos"
    >
      <div class="container">
        <div class="row">
          <div class="col">
            <ChartCircleTwo
              color="pinot"
              sectionProgress="100"
              circleValue="11"
              class="section-space--mb_40"
            />
          </div>
        </div>
        <SectionTitle
          color="pinot"
          sectionTitle="Listado de principales proyectos"
          class="wow move-up"
        />
      </div>
    </div>
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
import NuestraMision from "@/components/NuestraMision";
import QuienesSomos from "@/components/QuienesSomos";
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
  },
};
</script>

