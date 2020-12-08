<template>
  <div>
    <div class="mb-5 intro blue">
      <strong>4 Tesis de posgrado </strong> con base en proyectos de I+D del
      centro:
    </div>
    <div v-for="tesis in list" :key="tesis.id">
      <h6>{{ tesis.authors }}</h6>
      <h3>
        <strong>{{ tesis.title }}</strong>
      </h3>
    </div>
  </div>
</template>
<script>
export default {
  name: "Anexo4",
  data: () => ({
    list: [
      {
        id: "tesis-1",
        authors: "Richard Bustos y Wladimir Esteban",
        type: "Tesis de Magister",
        title:
          "EVALUACIÓN DEL MÉTODO DE RENOVACIÓN SUPERFICIAL PARA ESTIMAR FLUJOS DE CALOR LATENTE SOBRE UN VIÑEDO (cv. Cabernet sauvignon) REGADO POR GOTEO",
        grade: "Magister en hortofruticultura",
        other: "Asociados a proyecto “Surface renewal”",
      },
      {
        id: "tesis-2",
        authors: "Felipe Saez",
        type: "Tesis de Magister",
        title:
          "Desarrollo de un método de detección de Botryosphaeriaceae asociadas a la enfermedad de la madera de Vitis vinifera basado en PCR isotérmico",
        grade: "Magister en Biotecnología",
        other:
          "Asociado a proyecto “Microbial diagnostics using Omic-Based Technologies”",
      },
      {
        id: "tesis-3",
        authors: "Claudio Urra",
        type: "Tesis de Doctorado",
        title:
          "Caracterización de la variabilidad genética de los clones de las variedades de Vitis vinifera utilizadas por las viñas chilenas",
        grade: "Doctor en Biotecnología",
        other: "Asociado a proyecto “Whole Genome Analytics”",
      },
      {
        id: "tesis-4",
        authors: "Jaime Alarcón",
        type: "",
        title:
          "Determinación de la influencia de sequía en la respuesta molecular de Araucaria araucana frente a la inoculación de microorganismos patógenos asociados al daño foliar",
        grade: "Dr (c) en Biociencias moleculares",
        other:
          "Asociado a proyecto “Desarrollo e implementación de herramientas genómicas para el manejo del Daño Foliar de Araucaria araucana y su relación con prácticas culturales de conservación”",
      },
    ],
  }),
};
</script>
<style lang="scss" scoped>
.title-unit {
  font-size: 25px;
  margin-bottom: 20px;
}
</style>