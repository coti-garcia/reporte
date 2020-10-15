<template>
  <div
    class="feature-app-showcase section-space--pt_120 section-space--mb_120"
    id="presentacion"
  >
    <div class="container">
      <div class="row">
        <div class="col">
          <ChartCircleTwo
            circleValue="01"
            class="section-space--mb_40"
            color="arboretum"
            sectionProgress="10"
          />
        </div>
      </div>
      <SectionTitle
        color="arboretum"
        sectionTitle="Presentación"
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
  name: "Presentacion",
  components: {
    SectionTitle,
    ServiceAgency,
    ChartCircleTwo,
    FeatureApp,
  },
};
</script>

<style lang="scss" scoped>
</style>