<template>
  <div class="row px-4">
    <div
      class="ht-team-member col-6 col-md-3 col-lg-2 mb-4 wow move-up"
      v-for="item in team"
      :key="item.name"
    >
      <TeamMember
        :name="item.name"
        :boardPosition="item.boardPosition"
        :position="item.position"
        :img="`http://via.placeholder.com/500x500`"
        :country="item.country"
      />
    </div>
    <!-- ht-team-member End -->
    <div class="col-12">
      <h4 class="arboretum font-weight--light mb-15 wow move-up">
        PAST DIRECTORS
      </h4>
    </div>
    <div
      class="ht-team-member col-6 col-md-3 col-lg-2 mb-4 wow move-up"
      v-for="(item, i) in pastTeam"
      :key="i"
    >
      <TeamMember
        :name="item.name"
        :position="item.position"
        :country="item.country"
      />
    </div>
  </div>
</template>

<script>
import TeamMember from "@/components/TeamMember";
export default {
  name: "TeamTwo",
  components: {
    TeamMember,
  },
  data() {
    return {
      team: [
        {
          boardPosition: "Presidente",
          name: "Cindy M. Kiel",
          position:
            "Excecutive Associate Vice Chancellor of Research Administration",
          img: "",
          country: "US",
        },
        {
          boardPosition: "Vice-Presidente",
          name: "Joanna Regulska",
          position: "Vice Provost and Dean of Global Affairs",
          img: "",
          country: "US",
        },
        {
          boardPosition: "Secretaria",
          name: "Kristen C. Stevenson",
          position: "Associate Campus Counsel",
          img: "",
          country: "US",
        },
        {
          boardPosition: "Director",
          name: "William Tucker",
          position:
            "Associate Vice Chancellor for Innovation and Technology Commercialization",
          img: "",
          country: "US",
        },
        {
          boardPosition: "Director",
          name: "Prasant Mohapatra",
          position: "Vice Chancellor for Research",
          img: "",
          country: "US",
        },
        {
          boardPosition: "Director",
          name: "Ermias Kebreab",
          position:
            "Associate Vice Provost of Academic Programs in Global Affairs",
          img: "",
          country: "US",
        },
        {
          boardPosition: "Director",
          name: "Michael Lazzara",
          position: "Associate Vice Provost of Academic Programs.",
          img: "",
          country: "US",
        },
        {
          boardPosition: "Director",
          name: "Paul Dodd",
          position:
            "Associate Vice Chancellor for Interdisciplinary Research and Strategic Initiatives, UC Davis",
          img: "",
          country: "US",
        },
        {
          boardPosition: "Director",
          name: "Pedro Bustos",
          position:
            "Director Nacional del Instituto de Investigaciones Agropecuarias (INIA), en representación del Ministerio de Agricultura",
          img: "",
          country: "CL",
        },
        {
          boardPosition: "Director",
          name: "Pablo Villalobos",
          position:
            "Director Departamento de Innovación y Transferencia Tecnológica, Universidad de Tarapacá",
          img: "",
          country: "CL",
        },
        {
          boardPosition: "Director",
          name: "Eugenio Doussoulin",
          position: "Associate Campus Counsel",
          img: "",
          country: "CL",
        },
        {
          boardPosition: "Director",
          name: "Ariel Orellana",
          position:
            "Vicerrector de Investigación y Doctorado, Universidad Andrés Bello",
          img: "",
          country: "CL",
        },
      ],
      pastTeam: [
        {
          name: "Cameron Carter",
          position: "Presidential Chair in Neuroscience",
          img: "",
          country: "US",
        },
        {
          name: "James Hill",
          position:
            "Associate Dean for International Programs in the College of Agricultural and Environmental Sciences",
          img: "",
          country: "US",
        },
        {
          name: "Dushyant Pathak",
          position:
            "Former Associate Vice Chancellor of Technology Management and Corporate Relations",
          img: "",
          country: "US",
        },
        {
          name: "Harris Lewin",
          position: "Former Vice Chancellor for Research",
          img: "",
          country: "US",
        },
        {
          name: "Gonzalo Herrera",
          position:
            "Ex Vicerrector de Innovación, representante Universidad de Talca 2015-2017",
          img: "",
          country: "CL",
        },
        {
          name: "Julio Kalazich",
          position: "Director de INIA 2014-2018",
          img: "",
          country: "CL",
        },
      ],
    };
  },
};
</script>
