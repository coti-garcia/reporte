<template>
  <div
    class="applanding-ts testimonial-slider-area section-space--pt_120"
    id="testimonial"
  >
    <div class="testimonial-slider-area section-space--pb_90">
      <div class="container">
        <div class="row">
          <div class="col">
            <ChartCircleTwo circleValue="02" class="section-space--mb_40" />
          </div>
        </div>
        <SectionTitle
          sectionTitle="Cartas de presentación"
          class="wow move-up"
        />
        <div class="row">
          <div class="col-lg-12">
            <div
              class="testimonial-slider border-bottom-drak section-space--pb_90"
            >
              <div class="swiper-container testimonial-slider__container">
                <div class="swiper-wrapper testimonial-slider__wrapper">
                  <swiper :options="swiperOption">
                    <div class="swiper-slide wow move-up">
                      <div class="app-landing-testimonial-slider__wrap">
                        <div class="post-thumbnail">
                          <img
                            src="http://via.placeholder.com/500x500"
                            class="img-fluid"
                            alt=""
                          />
                        </div>
                        <div class="testimonial-slider--info">
                          <div class="testimonial-slider__text">
                            Lorem ipsum dolor sit amet, consetetur sadipscing
                            elitr, sed diam nonumy eirmod tempor invidunt ut
                            labore et dolore magna aliquyam erat, sed diam
                            voluptua. At vero eos et accusam et justo duo
                            dolores et ea rebum. Stet clita kasd gubergren, no
                            sea takimata sanctus est Lorem ipsum dolor sit amet.
                            Lorem ipsum dolor sit amet, consetetur sadipscing
                            elitr, sed diam nonumy eirmod tempor invidunt ut
                            labore et dolore magna aliquyam erat, sed diam
                            voluptua. At vero eos et accusam et justo duo
                            dolores et ea rebum. Stet clita kasd gubergren, no
                            sea takimata sanctus est Lorem ipsum dolor sit amet.
                            Lorem ipsum dolor sit amet, consetetur sadipscing
                            elitr, sed diam nonumy eirmod tempor invidunt ut
                            labore et dolore magna aliquyam erat, sed diam
                            voluptua. At vero eos et accusam et justo duo
                            dolores et ea rebum. Stet clita kasd gubergren, no
                            sea takimata sanctus est Lorem ipsum dolor sit amet.
                          </div>
                          <div class="testimonial-slider__author">
                            <h6 class="name">Mauricio Cañoles:</h6>
                            <span class="designation">xxxxxx</span>
                          </div>
                        </div>
                      </div>
                    </div>
                    <div class="swiper-slide wow move-up">
                      <div class="app-landing-testimonial-slider__wrap">
                        <div class="post-thumbnail">
                          <img
                            src="http://via.placeholder.com/500x500"
                            class="img-fluid"
                            alt=""
                          />
                        </div>
                        <div class="testimonial-slider--info">
                          <div class="testimonial-slider__text">
                            ” Their customer support was amazing. Their help was
                            quick and gave me very clear instructions to follow!
                            Thanks!”
                          </div>
                          <div class="testimonial-slider__author">
                            <h6 class="name">Abbie Ferguson</h6>
                            <span class="designation">WEB DESIGNER</span>
                          </div>
                        </div>
                      </div>
                    </div>
                    <div class="swiper-slide wow move-up">
                      <div class="app-landing-testimonial-slider__wrap">
                        <div class="post-thumbnail">
                          <img
                            src="http://via.placeholder.com/500x500"
                            class="img-fluid"
                            alt=""
                          />
                        </div>
                        <div class="testimonial-slider--info">
                          <div class="testimonial-slider__text">
                            ” Their customer support was amazing. Their help was
                            quick and gave me very clear instructions to follow!
                            Thanks!”
                          </div>
                          <div class="testimonial-slider__author">
                            <h6 class="name">Abbie Ferguson</h6>
                            <span class="designation">WEB DESIGNER</span>
                          </div>
                        </div>
                      </div>
                    </div>
                  </swiper>
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
import ChartCircleTwo from "../components/ChartCircleTwo";
import SectionTitle from "../components/SectionTitle";
export default {
  name: "TestimonialFour",
  components: {
    ChartCircleTwo,
    SectionTitle,
  },
  data() {
    return {
      swiperOption: {
        speed: 800,
        loop: true,
      },
    };
  },
};
</script>
