<template>
  <div>
    <div class="section-space--pt_120 bg-gray" id="uc-davis-chile">
      <div class="container mb-md-5 pb-md-5">
        <div class="row">
          <div class="col">
            <ChartCircleTwo
              circleValue="04"
              class="section-space--mb_40 section-space--mt_30"
              color="icing"
              sectionProgress="50"
            />
            <SectionTitle
              color="redbud"
              sectionTitle="Centro de Innovación <br />UC Davis Chile"
              class="wow move-up"
            />
            <h3 class="subtitle text-center mb-5 redbud text-uppercase">
              Nuestro propósito de instalación
            </h3>
            <p class="text-center intro blue mx-auto mb-5">
              El <em>Centro de Innovación UC Davis Chile</em>, fundación de
              derecho privado sin fines de lucro, se ha consolidado en el país
              como un centro de excelencia con foco prioritario en los desafíos
              del sector agroalimentario y las temáticas medioambientales.
            </p>
          </div>
        </div>
        <div class="row">
          <div class="col-12 col-md-6 mb-3">
            <img src="@/assets/img/UC-Davis-CL.png" width="100%" />
          </div>
          <div class="col-12 col-md-6">
            <p>
              Nuestra historia tiene raíces en esta relación de larga data entre
              Chile y California, la que se consolida definitivamente con la
              postulación y adjudicación en 2013 y lanzamiento en 2015, del
              <em
                >Programa de Atracción de Centros Internacionales de
                Excelencia</em
              >
              de CORFO.
            </p>
            <p>
              Parte de los anhelos y del modelo de trabajo de la Universidad de
              California, Davis están relacionados con el trabajo colaborativo
              entre la academia, la industria y el sector público. Es en ese
              sentido que Chile fue visto como un lugar donde es posible
              potenciar la investigación, aportar con las capacidades de UC
              Davis y obtener así un intercambio valioso de conocimientos e
              innovación en una red global.
            </p>
            <p>
              Con cinco años de vida, nuestro
              <em>Centro de Innovación UC Davis Chile</em>, se ha convertido en
              un verdadero puente que conecta la investigación, el desarrollo
              tecnológico y las innovaciones con aplicaciones concretas que
              crean valor público, privado, académico y empresarial.
            </p>
          </div>
        </div>
        <!-- product overview -->
      </div>
      <Timeline />
      <CifrasGestion />
      <div class="section-space--ptb_120 bg-image">
        <div class="container">
          <div class="row">
            <div class="col-12">
              <h3 class="subtitle mb-5 redbud text-uppercase">
                Mirando hacia la<br />
                <strong>sustentabilidad futura</strong>
              </h3>
            </div>
          </div>
          <div class="row">
            <div class="col-12 col-md-10 blue big-text">
              <p>
                La experiencia internacional conocida por todos, muestra que la
                investigación fundamental es normalmente financiada por fondos
                públicos, tanto a través de los fondos basales entregados a las
                universidades, como por proyectos individuales en los que éstas
                también participan. Así se genera gran parte de la producción
                científica de nuestra Universidad en California (el 2019, de los
                USD 845,5 millones obtenidos por UC Davis para I+D, más del 81%
                proviene del gobierno federal y del Estado de California).
              </p>
              <p>
                Distinto es el caso de centros con temáticas específicas, con un
                foco claro en la investigación aplicada y el desarrollo de
                tecnología y/o conocimiento destinado a su aplicación productiva
                o como bien público. Este el caso de los Centros de Excelencia
                Internacional que hoy funcionan en Chile y otros Centros
                Tecnológicos. En este caso el modelo apunta a un financiamiento
                de tres tercios: uno basal aportado por el Estado, otro de
                fondos públicos competitivos y el último de contratos
                específicos con la industria
              </p>
              <p>
                UC Davis Chile procura avanzar hacia este modelo, utilizando
                como base el conocimiento y la experiencia de la Universidad de
                California que se ha generado por la inversión del estado de
                California y fondos federales de los Estados Unidos, así como el
                conocimiento de nuestros socios académicos en Chile.
              </p>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import ChartCircleTwo from "@/components/ChartCircleTwo";
import SectionTitle from "@/components/SectionTitle";
import Timeline from "@/components/Timeline";
import CifrasGestion from "@/components/CifrasGestion";
export default {
  name: "UCDavisChile",
  components: {
    SectionTitle,
    ChartCircleTwo,
    Timeline,
    CifrasGestion,
  },
};
</script>

<style lang="scss" scoped>
.subtitle {
  font-size: 28px;
  @media #{$min-tablet} {
    font-size: 35px;
  }
}
.big-text {
  font-size: 18px;
}
</style>