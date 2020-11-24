<template>
  <section class="bg-white">
    <div class="container cifras section-space--ptb_120">
      <div class="row">
        <div class="col-12">
          <h3 class="subtitle text-center mb-5 redbud text-uppercase">
            CIFRAS DE NUESTRA GESTIÓN
          </h3>
        </div>
      </div>
      <div class="row section-space--pb_60">
        <div class="col-12 col-md-6">
          <p>
            La instalación del Centro UC Davis Chile fue apoyada financieramente
            por el Programa de Atracción de Centros de Excelencia
            Internacionales de I+D para la Competitividad 2.0” de CORFO. Este
            programa definió condiciones de subsidio a 8 años plazo de forma
            decreciente en 3 Fases:
          </p>
          <p>
            <strong>Fase 1:</strong> Implementación: subsidio de hasta 50% del
            costo total. (3 años)
          </p>
          <p>
            <strong>Fase 1:</strong> Implementación: subsidio de hasta 50% del
            costo total. (3 años)
          </p>
          <p>
            <strong>Fase 3:</strong> Consolidación: subsidio de hasta 25% del
            costo total. (2 años)
          </p>
          <p>
            La inversión completa en el Proyecto Centro de Excelencia
            Internacional UC Davis Chile es de aproximadamente
            <strong class="redbud">US$ 33 millones.</strong>
          </p>
        </div>
        <div class="col-12 col-md-6">
          <h5>Presupuesto Proyecto Centro de Excelencia Internacional</h5>
          <BudgetChart />
        </div>
      </div>
      <div class="row mt-5 section-space--pb_60">
        <div class="col-12 col-md-7">
          <h5>Ingresos del Centro:</h5>
          <div class="row">
            <div class="col-12 col-md-6">
              <h6>Fase Instalación 3 años (2015-2017)</h6>
              <DoughnutChartOne />
            </div>
            <div class="col-12 col-md-6">
              <h6>Fase Instalación 3 años (2018-2020)</h6>
              <DoughnutChartTwo />
            </div>
          </div>
        </div>
        <div class="col-12 col-md-5">
          <p>
            Durante estas dos fases del proyecto, el Centro UC Davis Chile ha
            logrado además generar ingresos a través de otras fuentes, más allá
            del subsidio del programa de Atracción de Centros de Excelencia
            Internacional, donde en los primeros 3 años de instalación estos
            recursos fueron un 2% de la operación total. Actualmente el proyecto
            se encuentra en su Fase 2 de Operación, en la cual se ha logrado que
            el 15% de la actividad sea financiada por proyectos fuera del
            Programa de Atracción de Centros de CORFO.
          </p>
        </div>
      </div>
      <div class="row section-space--ptb_60">
        <div class="col-12 col-md-6">
          <p>
            Desde el punto de vista de las acciones del Centro, reflejado en el
            gasto de los recursos, hemos tenido una evolución desde la Fase de
            Instalación a la Fase de Operación donde se destacan:
          </p>
          <ul>
            <li>Aumento de la eficiencia en Administración</li>
            <li>
              Mayor llegada a la aplicación de la Ciencia y el Conocimiento en
              la industria y la sociedad, a través de Transferencia Tecnológica
              y Extensión
            </li>
            <li>
              Fortalecimiento de las capacidades de I+D e Innovación de los
              socios estratégicos chilenos (Partnership)
            </li>
          </ul>
        </div>
        <div class="col-12 col-md-6">
          <h5>Gastos del Centro:</h5>
          <SpendChart />
        </div>
      </div>
    </div>
  </section>
</template>
<script>
import BudgetChart from "@/components/BudgetChart";
import SpendChart from "@/components/SpendChart";
import DoughnutChartOne from "./DoughnutChartOne.vue";
import DoughnutChartTwo from "./DoughnutChartTwo.vue";
export default {
  name: "CifrasGestion",
  components: {
    BudgetChart,
    SpendChart,
    DoughnutChartTwo,
    DoughnutChartOne,
  },
  data: () => ({}),
};
</script>
<style lang="scss" scoped>
.cifras {
  h5 {
    text-transform: uppercase;
    font-size: 17px;
    font-weight: bold;
    color: $blue;
    margin-bottom: 15px;
  }
  h6 {
    text-transform: uppercase;
    color: $blue;
    font-size: 15px;
    margin-bottom: 15px;
  }
}
</style>