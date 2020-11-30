<template>
  <div class="feature-app-showcase section-space--pt_120" id="presentacion">
    <div class="container">
      <div class="row">
        <div class="col">
          <ChartCircleTwo
            circleValue="01"
            class="section-space--mb_40"
            color="arboretum"
            sectionProgress="11"
          />
        </div>
      </div>
      <SectionTitle
        color="arboretum"
        sectionTitle="El sentido de este reporte"
        class="wow move-up"
      />
      <div class="row">
        <div class="col-12 col-md-3">
          <p class="intro blue">
            Con cinco años de vida, el
            <em>Centro de Innovación UC Davis Chile</em> presenta una
            recopilación de lo que han sido, hasta ahora, los principales
            resultados desde nuestra instalación en el país.
          </p>
        </div>
        <div class="col-12 col-md-4">
          <p>
            Nuestra llegada responde a un estrecho lazo de más de cinco décadas
            entre Chile y el estado de California, relación que se materializa
            en este Centro cuyo foco principal es contribuir desde la ciencia
            aplicada y la investigación y desarrollo al crecimiento y
            productividad del país, principalmente en el ámbito de la
            agroindustria, uno de los sectores prioritarios para Chile y en el
            que la Universidad de California Davis es líder mundial.
          </p>
          <p>
            Si bien en los inicios nos enfocamos en el sector de vitivinícola,
            al andar los años en UC Davis Chile hemos ampliado nuestro ámbito de
            acción, incorporando competencias en los rubros de alimentos y medio
            ambiente fortaleciendo el vínculo entre la ciencia y la industria en
            temáticas que tanto para Chile como para California se han vuelto de
            gran relevancia.
          </p>
        </div>
        <div class="col-12 col-md-4">
          <p>
            El propósito, vigente desde 2015 año en que se inauguró UC Davis
            Chile, lo definimos como el
            <em class="arboretum"
              >brindar soluciones tecnológicas basadas en ciencia al mercado y a
              la sociedad.</em
            >
            Sin embargo, más allá de ello, hemos sido protagonistas y testigos
            del impacto que este objetivo ha tenido en las comunidades y sobre
            todo en las personas. El compartir la experiencia de California con
            Chile ha sido tremendamente inspirador para quienes han sido parte y
            beneficiarios de los proyectos desarrollados en estos cinco años. No
            solo por los aprendizajes e incorporación de capacidades, sino por
            el sentido de tener la posibilidad de aplicarlos al servicio de
            Chile y desde Chile.
          </p>
          <p>
            Queremos compartir con ustedes nuestra experiencia e invitarlos a
            ser parte de los nuevos desafíos que en el Centro de Innovación UC
            Davis Chile pretendemos abordar, con el objetivo de seguir siendo
            una institución cuyo aporte está al servicio del país.
          </p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import SectionTitle from "@/components/SectionTitle";
import ChartCircleTwo from "@/components/ChartCircleTwo";
import FeatureApp from "@/components/FeatureApp";
export default {
  name: "Presentacion",
  components: {
    SectionTitle,
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