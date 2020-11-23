<template>
  <div
    class="feature-app-showcase section-space--pt_120 section-space--pb_120 bg-blue"
    id="proyectos"
  >
    <div class="container">
      <div class="row">
        <div class="col">
          <ChartCircleTwo
            color="cabernet"
            sectionProgress="100"
            circleValue="10"
            class="section-space--mb_40"
          />
        </div>
      </div>
      <SectionTitle
        color="white"
        sectionTitle="Principales Proyectos"
        class="wow move-up"
      />
    </div>
    <!-- portfolio item wrapper start -->
    <div class="portfolio-pages-wrapper">
      <div class="container">
        <div
          class="row clearfix masonry-wrap"
          v-masonry
          transition-duration="3s"
          item-selector=".masonary-item"
        >
          <div
            class="col-lg-4 col-md-6 masonary-item wow move-up"
            v-for="project in projects"
            :key="project.id"
          >
            <div class="portfolio-grid-caption mb-30">
              <router-link
                :to="{ name: 'ProjectDetail', params: { slug: project.slug } }"
                class="single-grid-caption"
              >
                <div v-if="project.thumb" class="single-portfolio__thumbnail">
                  <img
                    :src="require(`@/assets/img/projects/${project.thumb}`)"
                    :alt="project.name"
                    class="img-fluid border-radus-5"
                  />
                </div>
              </router-link>
              <div class="post-info">
                <div class="post-categories carbernet">
                  {{ project.title }}
                </div>
                <h5 class="post-title font-weight--bold">
                  <router-link
                    :to="{
                      name: 'ProjectDetail',
                      params: { slug: project.slug },
                    }"
                    >{{ project.name }}</router-link
                  >
                </h5>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
    <!-- portfolio item wrapper end -->

    <!-- footer section -->
  </div>
</template>

<script>
import HeaderElement from "@/components/HeaderElement";
import Breadcrumb from "@/components/Breadcrumb";
import FooterMain from "@/components/FooterMain";
import OffcanvasSearchBox from "@/components/OffcanvasSearchBox";
import OffCanvasMobileMenu from "@/components/OffCanvasMobileMenu";
import SectionTitle from "@/components/SectionTitle";
import ChartCircleTwo from "@/components/ChartCircleTwo";
import Projects from "@/store/projects.js";
export default {
  name: "PortfolioMasonry",
  components: {
    HeaderElement,
    Breadcrumb,
    FooterMain,
    OffcanvasSearchBox,
    OffCanvasMobileMenu,
    SectionTitle,
    ChartCircleTwo,
  },

  mounted() {
    if (typeof this.$redrawVueMasonry === "function") {
      this.$redrawVueMasonry();
    }

    this.onLoad();
  },

  methods: {
    async onLoad() {
      await this.sleep(950);
      this.$redrawVueMasonry();
    },
    sleep(ms) {
      return new Promise((resolve) => setTimeout(resolve, ms));
    },
  },

  data() {
    return {
      projects: Projects.list,
    };
  },
};
</script>

