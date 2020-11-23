<template>
  <div
    class="feature-app-showcase section-space--pt_60 section-space--mb_120 section-space--pb_60"
    id="quienes-somos"
  >
    <div class="container">
      <div class="row">
        <div class="col">
          <ChartCircleTwo
            color="arboretum"
            sectionProgress="72"
            circleValue="08"
            class="section-space--mb_40"
          />
        </div>
      </div>
      <SectionTitle
        color="arboretum"
        sectionTitle="Quiénes somos"
        class="wow move-up"
      />
    </div>

    <section class="board section-space--pb_120">
      <div class="container mt-5">
        <div class="row">
          <div class="col-lg-10">
            <div class="section-title section-space--mb_60">
              <h3
                class="subtitle arboretum font-weight--light mb-15 wow move-up"
              >
                DIRECTORIO
              </h3>
              <p class="wow move-up">
                La gestión que realizamos en UC Davis Chile cuenta con el
                respaldo y apoyo de un destacado directorio que incluye a las
                más altas autoridades del campus de Davis, así como a
                representantes de universidades chilenas que trabajan
                directamente con nuestro Centro y quienes sesionan con una
                periodicidad de XXXXX con el objetivo de abordar nuestris los
                desafíos y proyecciones así como también para conocer el estátus
                de los proyectos que desarrollamos en el país.
              </p>
              <p class="wow move-up">
                Actualmente nuestro directorio está integrado por:
              </p>
            </div>
          </div>
        </div>
      </div>
      <div class="container-fluid">
        <Board />
      </div>
    </section>

    <section
      class="bg-arboretum executive-team section-space--pb_120 section-space--pt_60 mt-6"
    >
      <div class="container mt-5 inner-section">
        <div class="row pt-5">
          <div class="col-lg-4">
            <div class="section-title section-space--mb_60">
              <h3
                class="subtitle text-white font-weight--light mb-15 wow move-up"
              >
                EQUIPO DIRECTIVO
              </h3>
              <p class="wow move-up text-white">
                El equipo responsable del manejo y dirección del Centro de
                Innovación en Ciencias de la Vida UC Davis Chile actualmente
                está liderado por:
              </p>
            </div>
          </div>

          <div class="col-lg-8 px-4 justify-content-center">
            <div class="row">
              <div
                class="ht-team-member col-6 col-lg-4 mb-4 wow move-up"
                v-for="(item, e) in executiveTeam"
                :key="e"
              >
                <TeamMember
                  :name="item.name"
                  :position="item.position"
                  :img="`http://via.placeholder.com/500x500`"
                />
              </div>
            </div>
            <!-- ht-team-member End -->
          </div>
        </div>
        <div class="row mt-5">
          <div class="col-lg-4">
            <p class="wow move-up text-white">
              La estructura organizacional de nuestro Centro puede graficar de
              la siguiente manera:
            </p>
          </div>
          <div class="col-lg-8">
            <img
              src="http://via.placeholder.com/1500x700"
              alt="organization chart"
              class="img-fluid"
            />
          </div>
        </div>
      </div>
    </section>

    <section class="administration section-space--pt_60">
      <div class="container">
        <div class="row pt-5 mt-5">
          <div class="col-lg-10">
            <div class="section-title section-space--mb_60">
              <h3
                class="subtitle arboretum font-weight--light mb-15 wow move-up"
              >
                ADMINISTRACIÓN
              </h3>
              <p class="wow move-up">
                Para lograr el óptimo funcionamiento de UC Davis Chile, nuestro
                Centro cuenta con un equipo ejecutivo de alto nivel compuesto
                por especialistas de distintas áreas.
              </p>
              <p class="wow move-up">
                Actualmente nuestra administración cuenta con los siguientes
                profesionales:
              </p>
            </div>
          </div>
        </div>
      </div>
      <div class="container-fluid">
        <!-- <div class="row px-4 justify-content-center">
          <div
            class="ht-team-member col-6 col-md-3 col-lg-2 mb-4 wow move-up"
            v-for="(item, e) in administrativeTeam"
            :key="e"
          >
            <TeamMember
              :name="item.name"
              :position="item.position"
              :img="`http://via.placeholder.com/500x500`"
            />
          </div>
  
        </div> -->
        <div class="row">
          <div class="col-lg-12">
            <div class="swiper-container team-slider__container">
              <swiper :options="swiperOption">
                <div
                  class="swiper-slide"
                  v-for="(item, e) in administrativeTeam"
                  :key="e"
                >
                  <div class="grid-item wow move-up py-4">
                    <!-- ht-team-member Start -->
                    <div class="ht-team-member text-center">
                      <TeamMember
                        :name="item.name"
                        :position="item.position"
                        :img="`http://via.placeholder.com/500x500`"
                      />
                    </div>
                    <!-- ht-team-member End -->
                  </div>
                </div>
              </swiper>
              <!-- Add Arrows -->
              <div class="swiper-pagination section-space--mt_50"></div>
            </div>
          </div>
        </div>
      </div>
    </section>

    <section>
      <div class="container">
        <div class="row pt-5 mt-5">
          <div class="col-lg-10">
            <div class="section-title section-space--mb_60">
              <h3
                class="subtitle arboretum font-weight--light mb-15 wow move-up"
              >
                ESPECIALISTAS E INVESTIGADORES
              </h3>
              <p class="wow move-up">
                El Centro de Innovación en Ciencias de la Vida UC Davis Chile
                está integrado por especialistas e investigadores de los
                distintos ámbitos que componen el sector agroalimentario cuyo
                objetivo es desarrollar investigación colaborativa entre Chile y
                California, transferir tecnologías desarrolladas en los Estados
                Unidos hacia la industria chilena e instalar capacidades de UC
                Davis en Chile.
              </p>
              <p class="wow move-up">
                Profesionales investigadores y especialistas en agronomía,
                sustentabilidad, ciencias de la alimentación, vitivinicultura y
                enología, extención e innovación forman parte de nuestroequipo
                de excelencia el que actualmente está compuesto por:
              </p>
            </div>
          </div>
        </div>
      </div>
      <div class="container-fluid">
        <div class="row px-4 justify-content-center">
          <div
            class="ht-team-member col-6 col-md-3 col-lg-2 mb-4 wow move-up"
            v-for="(item, e) in researchTeam"
            :key="e"
          >
            <TeamMember
              :name="item.name"
              :position="item.position"
              :img="`http://via.placeholder.com/500x500`"
            />
          </div>
          <!-- ht-team-member End -->
        </div>
      </div>
    </section>
  </div>
</template>
<script>
import SectionTitle from "@/components/SectionTitle";
import ChartCircleTwo from "@/components/ChartCircleTwo";
import Board from "@/components/Board";
import TeamMember from "@/components/TeamMember";
export default {
  name: "QuienesSomos",
  components: {
    ChartCircleTwo,
    SectionTitle,
    Board,
    TeamMember,
  },
  data: () => ({
    swiperOption: {
      speed: 800,
      loop: false,
      slidesPerView: 6,
      spaceBetween: 30,
      pagination: {
        el: ".swiper-pagination",
        clickable: true,
      },
      breakpoints: {
        1499: {
          slidesPerView: 5,
        },

        991: {
          slidesPerView: 6,
        },

        767: {
          slidesPerView: 3,
        },

        575: {
          slidesPerView: 2,
        },
      },
    },
    executiveTeam: [
      {
        name: "Mauricio Cañoles",
        position: "General Manager",
        img: "",
        country: "CL",
      },
      {
        name: "Dario Cantu",
        position: "Academic Director",
        img: "",
        country: "CL",
      },
      {
        name: 'Lovell "Tu" Jarvis',
        position: "Executive Director",
        img: "",
        country: "CL",
      },
    ],
    administrativeTeam: [
      {
        name: "María Trinidad Eva",
        position: "Administration and Finance Manager",
        img: "",
      },
      {
        name: "Francisco Díaz",
        position: "Partnership and Communications Manager",
        img: "",
      },
      {
        name: "Jorge Cabezas",
        position: "Administration and Finance Coordinator",
        img: "",
      },
      {
        name: "Rodrigo Riquelme",
        position: "Partnership Coordinator",
        img: "",
      },
      {
        name: "Marcela Hidalgo",
        position: "Finance & Human Resources Analyst",
        img: "",
      },
      {
        name: "Patricio Cabezas",
        position: "Financial Assistant",
        img: "",
      },
      {
        name: "Silvia Fuentes ",
        position: "Executive Assistant",
        img: "",
      },
      {
        name: "Fernanda Retamales",
        position: "Finance Assistant",
        img: "",
      },
      {
        name: "Gabriela Jiménez",
        position: "Partnership Assistant",
        img: "",
      },
    ],
    researchTeam: [
      {
        name: "Alejandra Acuña",
        position: "Agronomy Coordinator",
        img: "",
      },
      {
        name: "Patricia Anguita",
        position: "Intelectual Property and Technology Transfer Coordinator",
        img: "",
      },
      {
        name: "Álvaro Castro",
        position: "Research and Development Coordinator",
        img: "",
      },
      {
        name: "Fernando Coz",
        position: "Environment and Sustainability Coordinator",
        img: "",
      },
      {
        name: "Leticia Rojas",
        position: "Innovation and Extension Coordinator",
        img: "",
      },
      {
        name: "Olivia Valdés",
        position: "Food Science Coordinator",
        img: "",
      },
      {
        name: "Jessica Alvarado",
        position: "Innovation and Extension Specialist",
        img: "",
      },
      {
        name: "Juan Carlos Galaz",
        position: "Innovation and Extension Specialist",
        img: "",
      },
      {
        name: "Victor González",
        position: "Innovation and Extension Specialist",
        img: "",
      },
      {
        name: "Natalia Díaz",
        position: "Innovation and Extension Specialist",
        img: "",
      },
      {
        name: "Camila Saavedra",
        position: "Viticulture and Enology Specialist",
        img: "",
      },
      {
        name: "Denise Cifuentes",
        position: "Bioprocess Researcher",
        img: "",
      },
      {
        name: "Patricio Muñoz",
        position: "Bioproduct Researcher",
        img: "",
      },
      {
        name: "Catalina Pavez",
        position: "Molecular Researcher",
        img: "",
      },
      {
        name: "Isidora Silva",
        position: "Junior Researcher",
        img: "",
      },
    ],
  }),
};
</script>
<style lang="scss" scoped>
.subtitle {
  text-transform: uppercase;
  font-size: 35px;
  font-weight: 300;
  margin-bottom: 20px;
}

// .executive-team {
//   transform: skewY(-6deg);
//   .inner-section {
//     transform: skewY(6deg);
//   }
//   z-index: -2;
// }
.board {
  z-index: 200;
}
.swiper-pagination.swiper-pagination-2
  .swiper-pagination-bullet-active::before {
  background: $arboretum;
}
</style>