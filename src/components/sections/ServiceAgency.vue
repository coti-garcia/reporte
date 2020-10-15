<template>
  <div class="digital-agency-assistance-area" id="about">
    <div class="container">
      <div class="row">
        <div class="col-lg-12">
          <div
            class="digital-agency-section-title text-center section-space--mb_60"
          >
            <h3 class="section-title font-weight--light mb-15 wow move-up">
              Lorem, ipsum dolor sit amet consectetur<br />consectetur
              adipisicing elit.
            </h3>
          </div>
        </div>
      </div>

      <!-- service agency component -->
      <ServiceItemAgency />
    </div>
  </div>
</template>

<script>
import ServiceItemAgency from "../ServiceItemAgency";
export default {
  name: "ServiceAgency",
  components: {
    ServiceItemAgency,
  },
};
</script>

<style lang="scss">
</style>