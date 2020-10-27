<template>
  <div class="ht-tab-wrap">
    <b-tabs class="ht-tab-menu">
      <b-tab title="Objetivos" active>
        <!-- tab content one component -->
        <!-- <TabContentOne /> -->
      </b-tab>
      <b-tab title="Valores">
        <!-- tab content two component -->
        <Valores />
      </b-tab>
      <b-tab title="Misión (Propósito)">
        <!-- tab content third component -->
        <div class="clinic-work-process-step section-space--pt_90">
          <div class="row">
            <div class="col-lg-6">
              <div class="clinic-work-step__media images-left-ml text-center">
                <img
                  src="../assets/img/features/aeroland-clinic-image-01.png"
                  class="img-fluid"
                  alt="thumbnail"
                />
              </div>
            </div>
            <div class="col-lg-5">
              <div class="clinic-work-process-step__content">
                <div class="app-showcase__inner">
                  <div class="sub__title mb-20">
                    <h6 class="font-weight--blod">Misión</h6>
                  </div>
                  <h4 class="font-weight--bold">Propósito</h4>
                  <div class="sub-text section-space--mb_40">
                    <p>
                      Entregar al mercado y la sociedad soluciones tecnológicas
                      basadas en ciencia, a través de investigación
                      colaborativa, desarrollo y transferencia de tecnologías
                      que generen impacto económico y desarrollo social.
                    </p>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </b-tab>
      <b-tab title="Visión">
        <div class="clinic-work-process-step section-space--pt_90">
          <div class="row">
            <div class="col-lg-6 order-lg-1 order-2 wow move-up">
              <div class="clinic-work-process-step__content">
                <div class="app-showcase__inner">
                  <div class="sub__title mb-20">
                    <h6 class="font-weight--blod">Visión</h6>
                  </div>
                  <h4 class="font-weight--bold">
                    Ser líder en Latinoamérica en investigación aplicada y
                    transferencia de soluciones tecnológicas en ciencias de la
                    vida.
                  </h4>
                </div>
              </div>
            </div>
            <div class="col-lg-5 order-lg-2 order-1 wow move-up">
              <div class="clinic-work-step__media images-right-mr text-center">
                <img
                  src="../assets/img/features/aeroland-clinic-image-02.png"
                  class="img-fluid"
                  alt="thumbnail"
                />
              </div>
            </div>
          </div>
        </div>
      </b-tab>
    </b-tabs>
  </div>
</template>

<script>
import TabContentOne from "@/components/TabContentOne";
import TabContentTwo from "@/components/TabContentTwo";
import TabContentThree from "@/components/TabContentThree";
import Valores from "@/components/Valores";

export default {
  name: "TabOne",
  components: {
    TabContentOne,
    TabContentTwo,
    TabContentThree,
    Valores,
  },
};
</script>

<style lang="scss">
#mision {
  .ht-tab-menu {
    .nav-tabs li a.active {
      background: $strawberry !important;
    }
  }
  .sub-text {
    p {
      font-size: 18px;
    }
  }
}
</style>