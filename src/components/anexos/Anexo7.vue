<template>
  <div>
    <div class="mb-5 intro blue">
      <strong>96 Eventos de difusión </strong> para presentar resultados del
      Centro y hacer disponible el conocimiento avanzado de California en
      múltiples temáticas de interés para el sector productivo, académico y
      público:
    </div>
    <div v-for="event in events" :key="event.year">
      <h6>{{ event.year }}</h6>
      <div>
        {{ event.list }}
      </div>
    </div>
  </div>
</template>
<script>
export default {
  name: "Anexo7",
  data: () => ({
    events: [
      {
        year: "2015",
        list: [
          {
            id: "1",
            title:
              "Innova BioBio/UDD Tech Transfer Workshop. Charla Translational Research & Public-Private Partnerships.",
            datePlace: "Pablo Zamora UDD, Concepción. Febrero", //Esto puede ser solo la fecha o fecha y lugar.
          },
          {
            id: "2",
            title:
              "Inauguración UC Davis Chile. Salón O'Higgins del Ministerio de Relaciones Exteriores",
            datePlace: "21 de abril",
          },
          {
            id: "3",
            title: "",
            datePlace: "",
          },
        ],
      },
      {
        year: "2016",
        list: [
          {
            id: "8",
            title: "",
            datePlace: "",
          },
          {
            id: "9",
            title: "",
            datePlace: "",
          },
        ],
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