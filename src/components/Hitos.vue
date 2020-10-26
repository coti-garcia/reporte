<template>
  <div
    class="app-landing--center-slider-wrapper bg-blue section-space--ptb_120"
  >
    <div class="app-landing-listing-title-wrap drak-area section-space--pt_60">
      <div class="container">
        <div class="row">
          <div class="col-lg-3">
            <div class="app-landing-title-contet">
              <div class="title-details_two wow move-up">
                <h2>Hitos</h2>
              </div>
            </div>
          </div>
          <div class="col-lg-6 wow move-up">
            <ul class="check-list green-check-list section-space--mb_50">
              <li class="list-item">61 premios nobel</li>
              <li class="list-item">
                Más de 240 divulgaciones de invenciones al año
              </li>
              <li class="list-item">
                950 patentes activas en EE. UU. y el mundo
              </li>
              <li class="list-item">
                Más de 164 solicitudes de patentes al año
              </li>
              <li class="list-item">
                Más de US$13 millones en ingresos por licencias al año
              </li>
              <li class="list-item">14 startups creadas entre 2018 y 2019</li>
            </ul>
          </div>

          <div class="col-lg-3">
            <div class="app-landing-title-contet">
              <div class="title-details_one wow move-up">
                <h2>US$8,1</h2>
                <h5>billones</h5>
              </div>
              <div class="subtitle wow move-up">
                de contribución anual <br />a la economía de California
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
  name: "Hitos",
};
</script>

<style lang="scss">
.app-landing--center-slider-wrapper {
  transform: skewY(-8deg);
  .app-landing-listing-title-wrap {
    transform: skewY(8deg);
  }
}
.app-landing-title-contet {
  display: flex;
  flex-direction: column;
  & .title-details_one {
    max-width: 287px;
    width: 100%;
    & h2 {
      font-size: 55px;
      line-height: 1.1;
      font-weight: 700;
    }
    & h5 {
      font-size: 18px;
      line-height: 2;
      letter-spacing: 5px;
      font-weight: 700;
      text-transform: uppercase;
      margin-bottom: 20px;
    }
  }
  .subtitle {
    color: #fff;
    font-size: 25px;
  }
  & .title-details_two {
    margin-left: 0px;
  }

  @media #{$tablet-device} {
    & .title-details_one {
      margin-bottom: 30px;
    }
  }
  @media #{$small-mobile} {
    & .title-details_one {
      text-align: left;
    }
    & .title-details_two {
      margin-top: 30px;
      margin-bottom: 30px;
      margin-left: 0px;
    }
  }
  @media #{$large-mobile} {
    & .title-details_two {
      margin-top: 30px;
      margin-bottom: 30px;
      margin-left: 0px;
    }
  }
}
</style>