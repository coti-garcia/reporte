<template>
  <div class="feature-app-landing" id="uc-devis-us">
    <section class="light-yellow section-space--ptb_120">
      <div class="container">
        <div class="row">
          <div class="col-12">
            <ChartCircleTwo
              color="cabernet"
              sectionProgress="22"
              circleValue="02"
              class="section-space--mb_40"
            />
          </div>

          <div class="col-12">
            <SectionTitle
              color="cabernet"
              sectionTitle="UC Davis EE. UU."
              class="wow move-up"
            />
            <p class="text-center intro cabernet mx-auto mb-5">
              Fundada en 1908, la Universidad de California, Davis, es la
              universidad más académicamente completa de la costa oeste y una de
              solo cinco universidades públicas en los Estados Unidos con una
              amplia trayectoria en salud humana, salud animal y ciencias
              agrícolas y ambientales.
            </p>
          </div>
        </div>
        <div class="row relative">
          <div class="col-12 col-md-4 uc-davis-images">
            <img src="@/assets/img/UC-Davis-US-1.jpg" class="img-responsive" />
            <img src="@/assets/img/UC-Davis-US-2.jpg" class="img-responsive" />
            <img src="@/assets/img/UC-Davis-US-3.jpg" class="img-responsive" />
          </div>
          <div class="bg-image"></div>
          <div class="col-12 col-md-8">
            <p class="pl-md-3">
              UC Davis es una universidad pública de investigación con concesión
              de tierras (Grant Land) y programas académicos de alto prestigio
              en cuatro facultades (Ciencias Agrícolas y Ambientales, Ciencias
              Biológicas, Ingeniería, y Letras y Ciencias), además de seis
              escuelas (Educación, Derecho, Administración, Medicina, Enfermería
              y Medicina Veterinaria). Tiene una matrícula de 39.629 estudiantes
              (a otoño de 2019), inscritos en más de 100 carreras pregrado y más
              de 100 programas de postgrado.
            </p>
            <p class="pl-md-3">
              UC Davis es internacionalmente conocida por su trabajo
              multidisciplinario para resolver los desafíos más apremiantes del
              mundo y por su compromiso con la expresión artística y cultural.
              Ganó US$941,2 millones en fondos de investigación patrocinados en
              2019-20 y contribuye más de US$8.100 millones a la economía de
              California cada año. Entre los numerosos rankings, US Davis es
              reconocida como la quinta mejor universidad pública de los Estados
              Unidos, primera en el mundo en Ciencias Veterinarias y segunda en
              el mundo en Agricultura y Ciencias veterinarias.
            </p>
            <p class="pl-md-3">
              En noviembre de 2020 la Universidad de California, Davis fue la
              única universidad norteamericana galardonada con el Premio Platino
              2020 Aprendizaje, Investigación y Compromiso Global Institucional,
              honor mas alto que entrega la Asociación de Universidades Públicas
              de EEUU (APLU; The Association of Public and Land-grant
              Universities) y que reconoce los últimos seis años de esfuerzos de
              UC Davis impulsando estrategias integrales e inclusivas vinculadas
              con el compromiso global, la investigación y el aprendizaje.
            </p>
            <p class="pl-md-3">
              Las iniciativas internacionales son parte fundamental del Plan
              Estratégico de UC Davis “To Boldly Go”, incluyendo el plan del
              campus “Global Education for All”, el cuál tiene por finalidad
              proporcionar al 100 por ciento de los estudiantes universitarios,
              graduados y profesionales oportunidades de aprendizaje global que
              les ayuden a crear una conciencia global, explorar la diversidad
              mundial y buscar una acción global.
            </p>
            <p class="pl-md-3">
              Además del reconocimiento de la APLU, este año UC Davis compartió
              el primer lugar entre las universidades de EE.UU. destacadas en
              cuanto a diversidad e internacionalización, asimismo se le otorgó
              el premio Simon por la Internacionalización Integral del Campus, y
              fue reconocida como una de las mejores universidades en cuanto a
              la formación de becarios Fulbright de EE.UU., becarios Gilman y
              voluntarios del Cuerpo de Paz.
            </p>
          </div>
        </div>
      </div>
    </section>
    <UCDavisFeature class="section-space--mb_80 section-space--ptb_120" />

    <Hitos />
    <Colaboracion />
  </div>
</template>

<script>
import SectionTitle from "@/components/SectionTitle";
import ChartCircleTwo from "@/components/ChartCircleTwo";
import FeatureApp from "@/components/FeatureApp";
import ServiceAgency from "@/components/sections/ServiceAgency";
import UCDavisFeature from "@/components/UCDavisFeature";
import CurveShape from "@/components/CurveShape";
import Hitos from "@/components/Hitos";
import Colaboracion from "@/components/Colaboracion";
import Diagonales from "@/components/sections/Diagonales";

export default {
  name: "UCDavisUS",
  components: {
    SectionTitle,
    ServiceAgency,
    ChartCircleTwo,
    FeatureApp,
    UCDavisFeature,
    CurveShape,
    Colaboracion,
    Hitos,
    Diagonales,
  },
};
</script>
<style lang="scss" scoped>
.light-yellow {
  background: #fff9e5;
  position: relative;
}
.uc-davis-images {
  z-index: 20;
  img {
    max-width: 100%;
    margin-bottom: 20px;
    margin-top: 10px;
  }
}
.relative {
  position: relative;
  .bg-image {
    background: $cabernet;
    width: 200px;
    height: 80%;
    display: block;
    position: absolute;
    z-index: 0;
    top: -20px;
    left: -80px;
  }
}
</style>
