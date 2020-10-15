<template>
  <div class="feature-list-progress d-block">
    <div class="app-showcase-progress__title">
      <div class="feature-list-progress__counter">
        <div class="circle-progress-wrapper">
          <div class="chart-progress">
            <div class="chart-progress__inner-wrapper">
              <div class="chart-progress__inner chart-progress__inner--blue">
                <vue-circle
                  :progress="75"
                  :size="160"
                  line-cap="round"
                  :fill="blue"
                  :thickness="4"
                  :start-angle="0"
                  :show-percent="false"
                >
                </vue-circle>
                <div class="chart-progress__inner-content">
                  <h4 class="chart-progress__inner-text">
                    <span class="chart-number"> {{ circleValue }} </span>
                  </h4>
                </div>
              </div>
            </div>
          </div>
          <div class="circle-design circle-design--blue one"></div>
          <div class="circle-design circle-design--blue two"></div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import VueCircle from "vue2-circle-progress/src/index.vue";

export default {
  components: {
    VueCircle,
  },
  data() {
    return {
      fill: { gradient: ["#fad961", "#f76b1c"] },
      blue: { gradient: ["#0047BA", "#022851"] },
    };
  },
  props: {
    circleValue: String,
  },
};
</script>
<style scoped>
.chart-progress__inner--blue {
  background-color: transparent;
  background-image: url(https://communicationsguide.ucdavis.edu/sites/g/files/dgvnsk6246/files/inline-images/Turquoise.png);
  background-size: 101%;
  background-repeat: no-repeat;
  background-position: center center;
}
.app-showcase-progress__title .chart-progress__inner-wrapper {
  padding: 10px;
}
</style>
