<template>
  <div>
    <div class="mb-5 intro blue">
      Más de <strong>70 investigadores</strong> nacionales han sido parte del
      staff del Centro.
    </div>
    <ul>
      <li v-for="member in list" :key="member.id" class="mb-1">
        {{ member.name }}, <em>{{ member.grade }}</em>
      </li>
    </ul>
  </div>
</template>
<script>
export default {
  name: "Anexo2",
  data: () => ({
    list: [
      {
        id: "1001",
        name: "Alejandra Acuña Estrella",
        grade: "PhD",
      },
      {
        id: "1002",
        name: "Alvaro Gonzalo Castro Oyarzun",
        grade: "PhD",
      },
      {
        id: "1003",
        name: "",
        grade: "",
      },
      {
        id: "1004",
        name: "",
        grade: "",
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