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
    <Impacto />

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
import OverlayMenu from "@/components/OverlayMenu";
import NuestraMision from "@/components/sections/NuestraMision";
import QuienesSomos from "@/components/sections/QuienesSomos";
import AreasTrabajo from "@/components/sections/AreasTrabajo.vue";
import Proyectos from "@/components/sections/Proyectos.vue";
import Impacto from "@/components/sections/Impacto.vue";
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

    OverlayMenu,
    QuienesSomos,
    NuestraMision,
    AreasTrabajo,
    Proyectos,
    FooterMain,
    UCDavisChile,
    Impacto,
  },
};
</script>

