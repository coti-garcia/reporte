<template>
  <div>
    <div class="mb-5 intro blue">
      Más de <strong>85 Investigadores</strong>, académicos y staff de la
      Universidad de California Davis colaborando activamente en proyectos de
      I+D y extensión tecnológica:
    </div>
    <div v-for="item in researchers" :key="item.title" class="mb-5">
      <h2 class="text-uppercase gold title-unit">
        {{ item.title }}
      </h2>
      <table class="table table-striped">
        <thead>
          <tr>
            <th scope="col">UC Davis Unit</th>
            <th scope="col">Faculty/Staff Name</th>
            <th scope="col">Position at UC Davis</th>
          </tr>
        </thead>
        <tbody>
          <tr v-for="member in item.staff" :key="member.id">
            <td>{{ member.unit }}</td>
            <td>{{ member.name }}</td>
            <td>{{ member.position }}</td>
          </tr>
        </tbody>
      </table>
    </div>
  </div>
</template>
<script>
export default {
  name: "Anexo1",
  data: () => ({
    researchers: [
      {
        title: "College of Agricultural and Environmental Sciences",
        staff: [
          {
            id: "staff-1",
            unit: "Agricultural and Resource Economics Department",
            name: "Daniel Sumner, Ph.D.",
            position:
              "Director Agricultural Issues Center Frank H. Buck, Jr. Distinguished Professor Agricultural and Resource Economics",
          },
          {
            id: "staff-2",
            unit: "Food Science and Technology Department",
            name: "Bruce German Ph.D. ",
            position:
              "Professor and Chemist Department Food science and Technology Director, Foods For Health Institute",
          },
          {
            id: "staff-3",
            unit: "Food Science and Technology Department",
            name: "Christopher Simmons Ph.D",
            position:
              "Associate Professor Food Science and Technology Department",
          },
          {
            id: "staff-4",
            unit: "Food Science and Technology Department",
            name: "Edward (Ned) Spang Ph.D.",
            position:
              "Food science and Technology; Faculty lead Food Loss and Waste Collaborative",
          },
          {
            id: "staff-5",
            unit: "Food Science and Technology Department",
            name: "Linda Harris, Ph. D. ",
            position:
              "Chair Department of Food Science and Technology, College of Agricultural and Environmental Sciences, UC Davis",
          },
          {
            id: "staff-6",
            unit: "Food Science and Technology Department",
            name: "Moshe Rosenberg, Ph.D.",
            position:
              "Professor and Specialist, Dairy Engineering and Technology, Food Science and Technology Department",
          },
          {
            id: "staff-7",
            unit: "Human Ecology Department",
            name: "David de la Peña Ph.D.  ",
            position:
              "Program Director Landscape Architecture + Environmental Design; Human Ecology Department, College of agricultural & environmental Sciences",
          },
          {
            id: "staff-8",
            unit: "Land, air and water resources Department",
            name: "Ben Houlton Ph.D. ",
            position: "",
          },
          {
            id: "staff-9",
            unit: "",
            name: "",
            position: "",
          },
          {
            id: "staff-10",
            unit: "",
            name: "",
            position: "",
          },
          {
            id: "staff-11",
            unit: "",
            name: "",
            position: "",
          },
          {
            id: "staff-12",
            unit: "",
            name: "",
            position: "",
          },
          {
            id: "staff-13",
            unit: "",
            name: "",
            position: "",
          },
          {
            id: "staff-14",
            unit: "",
            name: "",
            position: "",
          },
          {
            id: "staff-15",
            unit: "",
            name: "",
            position: "",
          },
        ],
      },
      {
        title: "College of Engineering ",
        staff: [
          {
            id: "staff-101", //continua la numeración anterior, o le agregas un 1 al principio
            unit: "Agricultural and Resource Economics Department",
            name: "Daniel Sumner, Ph.D.",
            position:
              "Director Agricultural Issues Center Frank H. Buck, Jr. Distinguished Professor Agricultural and Resource Economics",
          },
          {
            id: "staff-2",
            unit: "Food Science and Technology Department",
            name: "Bruce German Ph.D. ",
            position:
              "Professor and Chemist Department Food science and Technology Director, Foods For Health Institute",
          },
        ],
      },
      {
        title: "College of Letters and Science",
        staff: [
          {
            id: "staff-201", //continua la numeración anterior, o le agregas un 2 al principio
            unit: "Agricultural and Resource Economics Department",
            name: "Daniel Sumner, Ph.D.",
            position:
              "Director Agricultural Issues Center Frank H. Buck, Jr. Distinguished Professor Agricultural and Resource Economics",
          },
          {
            id: "staff-2",
            unit: "Food Science and Technology Department",
            name: "Bruce German Ph.D. ",
            position:
              "Professor and Chemist Department Food science and Technology Director, Foods For Health Institute",
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
.table th,
.table td {
  max-width: 500px;
}
</style>