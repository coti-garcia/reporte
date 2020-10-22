<template>
  <div
    class="feature-app-landing bg-cabernet section-space--pt_120 section-space--mb_120"
    id="uc-devis-us"
  >
    <div class="container-fluid">
      <div class="row">
        <div class="col">
          <ChartCircleTwo
            color="cabernet"
            sectionProgress="30"
            circleValue="03"
            class="section-space--mb_40"
          />
        </div>
      </div>
      <SectionTitle
        color="white"
        sectionTitle="Universidad de California Davis "
        class="wow move-up"
      />
    </div>
    <UCDavisFeature class="section-space--mb_120" />
    <CurveShape class="no-height">
      <template v-slot:bgcolor>
        <path
          style="fill: #022851; stroke-miterlimit: 10"
          d="M3360.5,97.739c-242,0-480-48.375-480-48.375
                        S2647.5,0.5,2400.5,0.5s-480,48.375-480,48.375s-238,48.864-480,48.864s-480-48.375-480-48.375S727.5,0.5,480.5,0.5
                        S0.5,48.875,0.5,48.875V108h1920h1920V48.875C3840.5,48.875,3602.5,97.739,3360.5,97.739z"
        />
      </template>
    </CurveShape>
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
  },
};
</script>

