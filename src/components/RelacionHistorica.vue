<template>
  <div>
    <div
      class="app-showcase-process-wrapper section-space--pt_30"
      id="relacion-historica"
    >
      <div class="container">
        <div class="row">
          <div class="col">
            <ChartCircleTwo
              color="pinot"
              sectionProgress="40"
              circleValue="04"
              class="section-space--mb_40"
            />
          </div>
        </div>
      </div>

      <div class="app-showcase-section__titel">
        <div class="vc_row-separator center_curve bottom">
          <svg
            xmlns="http://www.w3.org/2000/svg"
            version="1.1"
            preserveAspectRatio="none"
            viewBox="0 0 100 100"
          >
            <path d="M 0 0 Q 50 200 100 0"></path>
          </svg>
        </div>
      </div>
    </div>
    <div class="app-showcase-step-wrap">
      <SectionTitle
        color="pinot"
        sectionTitle="Relación histórica"
        class="wow move-up"
      />
      <!-- App Showcase Process Step component -->
    </div>
  </div>
</template>

<script>
import ChartCircleTwo from "../components/ChartCircleTwo";
import SectionTitle from "../components/SectionTitle";
import ThreeStepProcess from "../components/ThreeStepProcess";
import AppShowcaseProcessStep from "../components/AppShowcaseProcessStep";
export default {
  name: "RelacionHistorica",
  components: {
    SectionTitle,
    ChartCircleTwo,
    ThreeStepProcess,
    AppShowcaseProcessStep,
  },
};
</script>

<style lang="scss" scoped>
.app-showcase-step-wrap {
  height: 500px;
}
</style>