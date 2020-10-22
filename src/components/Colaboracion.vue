<template>
  <div
    class="payment-staps-way-last_wrap dark-area section-space--pt_60 section-space--ptb_60"
  >
    <div class="container">
      <div class="row">
        <div class="col-lg-12">
          <div class="payment-process-step__three section-space--ptb_60">
            <div class="row align-items-center">
              <div
                class="col-lg-6 col-md-12 wow move-up"
                style="visibility: visible"
              >
                <div class="payment-process-step__media text-center">
                  <img
                    src="http://via.placeholder.com/1500x1000"
                    alt=""
                    class="img-fluid"
                  />
                </div>
              </div>
              <div
                class="col-lg-6 col-md-12 wow move-up"
                style="visibility: visible"
              >
                <div class="payment-process-step__content float-md-right">
                  <div class="payment-process__inner">
                    <h4 class="font-weight--blod section-space--mb_40">
                      Colaboración y extensionismo
                    </h4>
                    <div class="sub-text section-space--mb_20">
                      Desde sus inicios, UC Davis trabaja en conjunto con
                      instituciones públicas y privadas y pone énfasis en la
                      extensión y transferencia tecnológica.
                    </div>
                    <div class="sub-text section-space--mb_40">
                      En el área agroalimentaria, a cargo de la División de
                      Agricultura y Recursos Naturales, posee:
                    </div>
                    <div class="payment-conters section-space--mb_40">
                      <div class="row">
                        <div class="col-md-6 col-sm-6">
                          <div class="fun-fact--three">
                            <span class="fun-fact__count arboretum"
                              ><span>9</span></span
                            >
                            <h6 class="fun-fact__text white">
                              centros de investigación (Research and Extension
                              Centers) a lo largo de California
                            </h6>
                          </div>
                        </div>
                        <div class="col-md-6 col-sm-6">
                          <div class="fun-fact--three">
                            <span class="fun-fact__count arboretum"
                              ><span>130</span></span
                            >
                            <h6 class="fun-fact__text white">
                              especialistas en extensión cooperativa
                            </h6>
                          </div>
                        </div>
                        <div class="col-md-6 col-sm-6">
                          <div class="fun-fact--three">
                            <span class="fun-fact__count arboretum"
                              ><span>57</span></span
                            >
                            <h6 class="fun-fact__text white">oficinas</h6>
                          </div>
                        </div>

                        <div class="col-md-6 col-sm-6">
                          <div class="fun-fact--three">
                            <span class="fun-fact__count arboretum"
                              ><span>200</span></span
                            >
                            <h6 class="fun-fact__text white">asesores</h6>
                          </div>
                        </div>
                      </div>
                    </div>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Colaboracion",
};
</script>

<style lang="scss" scoped>
.dark-area {
  img {
    max-width: 100%;
  }
  color: #fff;
  .fun-fact--three {
    border-left: solid thin #fff;
    margin-bottom: 30px;
    padding-top: 0;
    span {
      line-height: 1;
    }
    &::before {
      display: none;
    }
  }
}
</style>