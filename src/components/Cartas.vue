<template>
  <div
    class="testimonial-slider-area section-space--ptb_120 bg-gray"
    id="testimonial"
  >
    <div class="container">
      <div class="row">
        <div class="col">
          <ChartCircleTwo circleValue="02" class="section-space--mb_40" />
        </div>
      </div>
      <div class="row">
        <div class="col-lg-12">
          <div class="section-title text-center section-space--mb_60">
            <h2 class="section-title font-width--light">
              Cartas de presentación
            </h2>
          </div>
          <div class="testimonial-slider">
            <div class="swiper-container testimonial-slider__container">
              <div class="swiper-wrapper testimonial-slider__wrapper">
                <swiper :options="swiperOption">
                  <div class="swiper-slide">
                    <div class="testimonial-slider__one">
                      <div class="testimonial-slider__text">
                        “Lorem ipsum dolor sit amet, consetetur sadipscing
                        elitr, sed diam nonumy eirmod tempor invidunt ut labore
                        et dolore magna aliquyam erat, sed diam voluptua. At
                        vero eos et accusam et justo duo dolores et ea rebum.
                        Stet clita kasd gubergren, no sea takimata sanctus est
                        Lorem ipsum dolor sit amet. Lorem ipsum dolor sit amet,
                        consetetur sadipscing elitr, sed diam nonumy eirmod
                        tempor invidunt ut labore et dolore magna aliquyam erat,
                        sed diam voluptua. At vero eos et accusam et justo duo
                        dolores et ea rebum. Stet clita kasd gubergren, no sea
                        takimata sanctus est Lorem ipsum dolor sit amet. Lorem
                        ipsum dolor sit amet, consetetur sadipscing elitr, sed
                        diam nonumy eirmod tempor invidunt ut labore et dolore
                        magna aliquyam erat, sed diam voluptua. At vero eos et
                        accusam et justo duo dolores et ea rebum. Stet clita
                        kasd gubergren, no sea takimata sanctus est Lorem ipsum
                        dolor sit amet.”
                      </div>
                      <div class="testimonial-slider--info">
                        <div class="post-thumbnail">
                          <img
                            src="http://via.placeholder.com/500x500"
                            class="img-fluid"
                            alt=""
                          />
                        </div>
                        <div class="testimonial-slider__author">
                          <h6 class="name">Mauricio Cañoles</h6>
                          <span class="designation">CARGO</span>
                        </div>
                      </div>
                    </div>
                  </div>
                  <div class="swiper-slide">
                    <div class="testimonial-slider__one">
                      <div class="testimonial-slider__text">
                        Lorem ipsum dolor sit amet, consetetur sadipscing elitr,
                        sed diam nonumy eirmod tempor invidunt ut labore et
                        dolore magna aliquyam erat, sed diam voluptua. At vero
                        eos et accusam et justo duo dolores et ea rebum. Stet
                        clita kasd gubergren, no sea takimata sanctus est Lorem
                        ipsum dolor sit amet. Lorem ipsum dolor sit amet,
                        consetetur sadipscing elitr, sed diam nonumy eirmod
                        tempor invidunt ut labore et dolore magna aliquyam erat,
                        sed diam voluptua. At vero eos et accusam et justo duo
                        dolores et ea rebum. Stet clita kasd gubergren, no sea
                        takimata sanctus est Lorem ipsum dolor sit amet. Lorem
                        ipsum dolor sit amet, consetetur sadipscing elitr, sed
                        diam nonumy eirmod tempor invidunt ut labore et dolore
                        magna aliquyam erat, sed diam voluptua. At vero eos et
                        accusam et justo duo dolores et ea rebum. Stet clita
                        kasd gubergren, no sea takimata sanctus est Lorem ipsum
                        dolor sit amet.Stet clita kasd gubergren, no sea
                        takimata sanctus est Lorem ipsum dolor sit amet. Lorem
                        ipsum dolor sit amet, consetetur sadipscing elitr, sed
                        diam nonumy eirmod tempor invidunt ut labore et dolore
                        magna aliquyam erat, sed diam voluptua. At vero eos et
                        accusam et justo duo dolores et ea rebum. Stet clita
                        kasd gubergren, no sea takimata sanctus est Lorem ipsum
                        dolor sit amet.”
                      </div>
                      <div class="testimonial-slider--info">
                        <div class="post-thumbnail">
                          <img
                            src="http://via.placeholder.com/500x500"
                            class="img-fluid"
                            alt=""
                          />
                        </div>
                        <div class="testimonial-slider__author">
                          <h6 class="name">Tu Jarvis</h6>
                          <span class="designation">CARGO</span>
                        </div>
                      </div>
                    </div>
                  </div>
                </swiper>
              </div>
            </div>
            <div
              class="swiper-pagination swiper-pagination-1 section-space--mt_60"
            ></div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import ChartCircleTwo from "../components/ChartCircleTwo";
import SectionTitle from "../components/SectionTitle";
export default {
  name: "Cartas",
  components: {
    ChartCircleTwo,
    SectionTitle,
  },
  data() {
    return {
      swiperOption: {
        speed: 800,
        loop: false,
        slidesPerView: 1,
        spaceBetween: 30,
        pagination: {
          el: ".swiper-pagination",
          clickable: true,
        },
        breakpoints: {
          1499: {
            slidesPerView: 1,
          },

          991: {
            slidesPerView: 1,
          },

          767: {
            slidesPerView: 1,
          },

          575: {
            slidesPerView: 1,
          },
        },
      },
    };
  },
};
</script>

<style lang="scss" scoped>
h2 {
  color: #022851;
}
.testimonial-slider__text {
  color: #333;
}
.post-thumbnail {
  .img-fluid {
    max-width: 100px;
    border-radius: 50%;
  }
}
</style>