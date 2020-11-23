<template>
  <div
    class="feature-app-landing bg-cabernet section-space--pt_120"
    id="uc-devis-us"
  >
    <div class="container-fluid">
      <div class="row">
        <div class="col">
          <ChartCircleTwo
            color="cabernet"
            sectionProgress="22"
            circleValue="02"
            class="section-space--mb_40"
          />
        </div>
      </div>
      <SectionTitle
        color="white"
        sectionTitle="UC Davis EE. UU."
        class="wow move-up"
      />
    </div>
    <UCDavisFeature class="section-space--mb_80" />

    <Hitos />
    <Colaboracion />
  </div>
</template>

<script>
import SectionTitle from "@/components/SectionTitle";
import ChartCircleTwo from "@/components/ChartCircleTwo";
import FeatureApp from "@/components/FeatureApp";
import ServiceAgency from "@/components/sections/ServiceAgency";
import UCDavisFeature from "@/components/UCDavisFeature";
import CurveShape from "@/components/CurveShape";
import Hitos from "@/components/Hitos";
import Colaboracion from "@/components/Colaboracion";
import Diagonales from "@/components/sections/Diagonales";

export default {
  name: "UCDavisUS",
  components: {
    SectionTitle,
    ServiceAgency,
    ChartCircleTwo,
    FeatureApp,
    UCDavisFeature,
    CurveShape,
    Colaboracion,
    Hitos,
    Diagonales,
  },
};
</script>

