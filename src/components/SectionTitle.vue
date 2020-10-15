<template>
  <div class="row">
    <div class="col-lg-12">
      <div class="section-title-wrap text-center section-space--mb_60">
        <h2 class="font-weight--bold mb-15 wow move-up" :class="color">
          {{ sectionTitle }}
        </h2>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "SectionTitle",
  props: {
    sectionTitle: String,
    color: String,
  },
};
</script>

<style lang="scss" scoped>
h2.font-weight--bold.mb-15.wow.move-up.cabernet {
  color: $cabernet;
}
</style>