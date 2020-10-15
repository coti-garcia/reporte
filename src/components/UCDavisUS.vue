<template>
  <div
    class="feature-app-showcase section-space--pt_120 section-space--mb_120"
    id="uc-devis-us"
  >
    <div class="container">
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
        color="cabernet"
        sectionTitle="UC Davis EE. UU."
        class="wow move-up"
      />
    </div>
  </div>
</template>

<script>
import SectionTitle from "../components/SectionTitle";
import ChartCircleTwo from "../components/ChartCircleTwo";
import FeatureApp from "../components/FeatureApp";
import ServiceAgency from "@/components/sections/ServiceAgency";
export default {
  name: "UCDavisUS",
  components: {
    SectionTitle,
    ServiceAgency,
    ChartCircleTwo,
    FeatureApp,
  },
};
</script>

