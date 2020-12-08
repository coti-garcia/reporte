<template>
  <div>
    <div class="mb-5 intro blue">
      <strong>30 Artículos </strong> de difusión técnica publicados en revistas
      especializadas del sector agroalimentario nacional:
    </div>
    <div v-for="article in articles" :key="article.id">
      {{ article }}
    </div>
  </div>
</template>
<script>
export default {
  name: "Anexo5",
  data: () => ({
    articles: [
      {
        id: "2001",
        date: "8/1/2020",
        title: "Fertil en microorganismos ",
        media: "Revista Mundo Agro",
        link: "https://www.mundoagro.cl/revistas/129/56/",
      },
      {
        id: "2002",
        date: "",
        title: "",
        media: "",
        link: "",
      },
      {
        id: "2003",
        date: "",
        title: "",
        media: "",
        link: "",
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