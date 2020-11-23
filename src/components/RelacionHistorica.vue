<template>
  <div>
    <div class="section-space--pt_120" id="relacion-historica">
      <div class="container">
        <div class="row">
          <div class="col">
            <ChartCircleTwo
              color="pinot"
              sectionProgress="33"
              circleValue="03"
              class="section-space--mb_40"
            />
            <SectionTitle
              color="pinot"
              sectionTitle="Relación histórica"
              class="wow move-up"
            />
            <p class="text-center intro pinot mx-auto mb-5">
              La decisión de instalar en Chile el Centro de Innovación en
              Ciencias de la Vida UC Davis, se enmarca dentro de una historia de
              más de 55 años de colaboración e intercambio académico entre Chile
              y California.
            </p>
          </div>
        </div>
        <div class="row">
          <div class="col-12 col-md-6">
            <p>
              A mediados de la década del 60, los respectivos gobiernos firmaron
              un acuerdo que se concretó con el envío de estudiantes y
              profesores desde la Universidad de Chile a la Universidad de Davis
              California.
            </p>
            <p>
              Ambas regiones presentan características climáticas, geográficas y
              variedades de especies animales y vegetales similares, en tanto
              que comparten desafíos en el cuidado de la biodiversidad, el
              manejo de cuencas hidrográficas y uso de energías. El desfase
              estacional, además, permite el intercambio comercial en el sector
              agrícola durante todo el año.
            </p>
            <p>
              A esta relación hoy se le atribuye gran parte del crecimiento de
              las exportaciones de uva y las frutas de carozo en Chile, e
              incluso el desarrollo de la industria de los vinos, en la que
              Chile se ha transformado en un importante actor a nivel mundial.
            </p>
          </div>
          <div class="col-12 col-md-6">
            <p>
              Los acuerdos de colaboración se han mantenido durante décadas y se
              han ido afianzando, con la conformación de comités, planes
              concretos e institucionalización de redes de trabajo y cooperación
              entre la academia y los sectores públicos y privados.
            </p>
            <p>
              En este marco, la asociación entre UC Davis y Chile permanece
              hasta el día de hoy con más de 60 estudiantes chilenos de posgrado
              e investigadores postdoctorales trabajando en los campus en
              California.
            </p>
            <p>
              En Chile, en tanto, gracias al Centro de Innovación en Ciencias de
              la Vida y la experiencia de UC Davis, la investigación agrícola ha
              movido sus fronteras con avanzadas técnicas genómicas, mientras
              que ha expandido sus campos de trabajo a otras áreas de
              investigación, con proyectos para la mitigación del cambio
              climático, manejo sustentable de cultivos, transferencia
              tecnológica, propiedad intelectual, medicina y planificación
              urbana, entre otras.
            </p>
          </div>
        </div>
        <!-- product overview -->
      </div>
      <ShowcaseRelacionHistorica />
      <div class="container">
        <div class="row icon-process-area section-space--ptb_120">
          <div class="col-lg-12">
            <h3 class="pinot text-center">Hitos desde los años 60 hasta hoy</h3>
            <Gradation />
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import ChartCircleTwo from "../components/ChartCircleTwo";
import SectionTitle from "../components/SectionTitle";
import ThreeStepProcess from "../components/ThreeStepProcess";
import AppShowcaseProcessStep from "../components/AppShowcaseProcessStep";
import ShowcaseRelacionHistorica from "@/components/ShowcaseRelacionHistorica.vue";
import Gradation from "../components/Gradation";
export default {
  name: "RelacionHistorica",
  components: {
    SectionTitle,
    ChartCircleTwo,
    ThreeStepProcess,
    AppShowcaseProcessStep,
    ShowcaseRelacionHistorica,
    Gradation,
  },
};
</script>

<style lang="scss" scoped>
.app-showcase-step-wrap {
  height: 500px;
}
.icon-process-area {
  h3 {
    padding-bottom: 60px;
  }
}
</style>