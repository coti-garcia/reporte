<template>
  <div class="digital-agency-grid">
    <a
      href="#"
      class="digital-agency-assistance__warap wow move-up"
      v-for="(item, index) in services"
      :key="index"
    >
      <div class="digital-agency-assistance__box">
        <div class="digital-agency-assistance__images">
          <div class="images-midea">
            <img :src="item.img" class="img-fluid" alt="service thumb" />
            <h5 class="heading">{{ item.heading }}</h5>
          </div>
        </div>
        <div class="digital-agency-assistance__content mt-30 text-center">
          <p>{{ item.desc }}</p>
        </div>
      </div>
    </a>
  </div>
</template>

<script>
export default {
  name: "ServiceItemAgency",
  data() {
    return {
      services: [
        {
          img: require("../assets/img/agency/agency-service-01.jpg"),
          heading: "Lorem ipsum dolor sit amet",
          desc:
            "Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua.",
        },
        {
          img: require("../assets/img/agency/agency-service-02.jpg"),
          heading: "Lorem ipsum dolor sit amet",
          desc:
            "Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua. ",
        },
        {
          img: require("../assets/img/agency/agency-service-03.jpg"),
          heading: "Lorem ipsum dolor sit amet",
          desc:
            "Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua. ",
        },
      ],
    };
  },
};
</script>

<style lang="scss">
</style>