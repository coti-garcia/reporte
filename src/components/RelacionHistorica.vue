<template>
  <div>
    <div class="section-space--ptb_120 bg-gray" id="relacion-historica">
      <div class="container">
        <div class="row">
          <div class="col">
            <ChartCircleTwo
              color="pinot"
              sectionProgress="40"
              circleValue="04"
              class="section-space--mb_40"
            />
            <SectionTitle
              color="pinot"
              sectionTitle="Relación histórica"
              class="wow move-up"
            />
          </div>
        </div>
      </div>
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