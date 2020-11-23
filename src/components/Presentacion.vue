<template>
  <div class="feature-app-showcase section-space--pt_120" id="presentacion">
    <div class="container">
      <div class="row">
        <div class="col">
          <ChartCircleTwo
            circleValue="01"
            class="section-space--mb_40"
            color="arboretum"
            sectionProgress="10"
          />
        </div>
      </div>
      <SectionTitle
        color="arboretum"
        sectionTitle="Presentación"
        class="wow move-up"
      />
      <h3 class="subtitle text-center arboretum">Para qué de este informe</h3>
      <div class="row">
        <div class="col-12 col-md-3">
          <p class="intro blue">
            Con cinco años de vida, el
            <em>Centro de Innovación en Ciencias de la Vida UC Davis Chile</em>
            presenta una recopilación de lo que han sido, hasta ahora, los
            principales resultados desde nuestra instalación en el país.
          </p>
        </div>
        <div class="col-12 col-md-4">
          <p>
            El surgimiento del centro UC Davis responde a un estrecho vinculo de
            más de cinco décadas entre los estados de Chile y California y que
            data de los años 60; una relación que se materializa en este Centro
            cuyo foco principal es contribuir desde la ciencia aplicada y la
            investigación y desarrollo al crecimiento y productividad del país,
            principalmente en el ámbito de la agroindustria, uno de los sectores
            prioritarios para Chile y en el que la Universidad de California
            Davis es líder mundial.
          </p>
          <p>
            Si bien en los inicios nos enfocamos en el sector de vitivinícola,
            al andar los años en UC Davis Chile hemos ampliado nuestro ámbito de
            acción incorporando competencias en los rubros de los alimentos y
            medio ambiente fortaleciendo el vínculo entre la ciencia y la
            industria en temáticas que tanto para Chile como para California se
            han vuelto de gran relevancia.
          </p>
        </div>
        <div class="col-12 col-md-4">
          <p>
            Como propósito, desde 2015 que en UC Davis Chile lo definimos como
            el brindar soluciones tecnológicas basadas en ciencia al mercado y a
            la sociedad, sin embargo, más allá de ello, hemos sido protagonistas
            y testigos del impacto que este propósito ha tenido en las
            comunidades y sobre todo en las personas. El compartir la
            experiencia de California con Chile ha sido tremendamente inspirador
            para quienes han sido parte y beneficiarios de los proyectos
            desarrollados en estos cinco años. No solo por los aprendizajes e
            incorporación de capacidades, sino por el sentido de tener la
            posibilidad de aplicar estos aprendizajes y capacidades al servicio
            de Chile, desde Chile.
          </p>
          <p>
            Queremos compartir con ustedes nuestra experiencia e invitarlos a
            ser parte de los nuevos desafíos del país que en el Centro de
            Investigación en Ciencias de la Vida UC Davis Chile pretendemos
            abordar con el objetivo de seguir siendo una institución cuyo aporte
            está al servicio del país.
          </p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import SectionTitle from "../components/SectionTitle";
import ChartCircleTwo from "../components/ChartCircleTwo";
import FeatureApp from "../components/FeatureApp";
import ServiceAgency from "@/components/sections/ServiceAgency";
export default {
  name: "Presentacion",
  components: {
    SectionTitle,
    ServiceAgency,
    ChartCircleTwo,
    FeatureApp,
  },
};
</script>

<style lang="scss" scoped>
.subtitle {
  text-transform: uppercase;
  font-size: 35px;
  font-weight: 300;
  margin-bottom: 50px;
  margin-top: -25px;
}
.intro {
  margin-bottom: 30px;
}
</style>