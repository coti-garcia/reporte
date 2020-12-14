<template>
  <div>
    <div class="mb-5 intro blue">
      <strong>96 Eventos de difusión </strong> para presentar resultados del
      Centro y hacer disponible el conocimiento avanzado de California en
      múltiples temáticas de interés para el sector productivo, académico y
      público:
    </div>
    <div class="row">
      <div v-for="event in events" :key="event.year" class="col-12">
        <ul class="timeline timeline-centered">
          <li class="timeline-item period">
            <div class="timeline-info"></div>
            <div class="timeline-marker"></div>
            <div class="timeline-content">
              <h2 class="timeline-title gold">{{ event.year }}</h2>
            </div>
          </li>

          <li v-for="item in event.list" :key="item.id" class="timeline-item">
            <div class="timeline-info">
              <span>{{ item.datePlace }}</span>
            </div>
            <div class="timeline-marker"></div>
            <div class="timeline-content">
              <p>{{ item.title }}</p>
            </div>
          </li>
        </ul>
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
            title:
              "Herramientas genómicas para la viticultura, Darío Cantu, investigador UC Davis. Auditorim Centro de Investigación e Innovación de Concha y Toro",
            datePlace: "3 de julio",
          },
          {
            id: "4",
            title:
              "Gestión de Propiedad Intelectual e Innovación, Dra. Mónica Alandete, UC Davis. Auditorim Centro de Investigación e Innovación de Concha y Toro",
            datePlace: "18 de agosto",
          },
          {
            id: "5",
            title:
              "Chile California Conference, Francisco Díaz, Partnership and Communications Manager en la U. de California, Davis.",
            datePlace: "17 de octubre",
          },
          {
            id: "6",
            title:
              'Charla magistral del Director Científico de UC Davis Chile, Pablo Zamora: "El uso de microbiomas para aplicaciones en agricultura" en evento de Lanzamiento Programa AgTech de RedAgrícola',
            datePlace: "Santiago 11 de diciembre de 2015.",
          },
          {
            id: "7",
            title:
              "Participación del Dr. Alan Bennett, Director Ejecutivo de UC Davis Chile, como expositor principal en el 2º Seminario de SaaS Generation, con la ponencia “Big Data in Agricultural Research”",
            datePlace: "14 de diciembre 2015",
          },
        ],
      },
      {
        year: "2016",
        list: [
          {
            id: "8",
            title:
              "Charla Magistral  en riego: “Towards next generation decision support for irrigation management” por los Investigadores de UC Davis, Dr. Rick Snyder y Dr. Daniele Zaccaría",
            datePlace: "Marzo 2016, Santiago y Talca.",
          },
          {
            id: "9",
            title:
              "Coferencia RedAgrícola Chile, Tres científicos de UC Davis Chile realizaron conferencias magistrales",
            datePlace: "1-2 de junio",
          },
          {
            id: "10",
            title:
              "Conferencia RedAgrícola Perú, Dos científicos de UC Davis Chile participaron como expertos invitados",
            datePlace: "22 y 23 de Junio",
          },
          {
            id: "11",
            title:
              "Charla “Impactando la agricultura de precisión: Herramientas metagenómicas para el diseño de bioproductos” Director Científico de UC Davis Chile – Pablo Zamora en Agro Planttrade",
            datePlace: "5 de octubre 2016",
          },
          {
            id: "12",
            title:
              "Participación de dos investigadores de UC Davis en el X Congreso Iberoamericano de Sensores, organizado por Universidad Federico Santa María. ",
            datePlace: "Ibersensor 2016",
          },
          {
            id: "13",
            title:
              "Seminario “Leading Technologies for Water Management” organizan CRHIAM/Universidad de Concepción/UC Davis Chile. Participan desde UC Davis: Dr. Jan Hopmans, Dr. Rick Snyder, Dr. Daniele Zaccaria.",
            datePlace: "Concepción, 24-26 octubre",
          },
          {
            id: "14",
            title:
              'Participación del Dr. Dusyhant Pathak como expositor destacado en el 4to encuentro "Chile: ciencia, tecnología y empresa" de CORFO.',
            datePlace: "26 octubre, Santiago",
          },
          {
            id: "15",
            title:
              "Taller de Riego: Surface Renewal: un método micro-meteorológico avanzado para medir evapotranspiración a nivel predial. coorganizado por UC Davis Chile y CRHIAM. taller dictado por los Investigadores de UC Davis: Dr. Rick Snyder y Dr. Daniele Zaccaría.",
            datePlace: "Chillán, 27-28 octubre",
          },
          {
            id: "16",
            title:
              "Seminario Internacional “Climate Smart Agro: Ciencia y Tecnologia para la Adaptacion Agroclimatica”. Organiza UC Davis Chile.",
            datePlace: "Santiago, 17 noviembre ",
          },
          {
            id: "17",
            title:
              "First Symposium on Food Safety (Universidad Andrés Bello y OCDE).",
            datePlace:
              "5 al 7 de diciembre, Casona Las Condes de la UNAB.Co-organiza UC Davis Chile",
          },
          {
            id: "18",
            title:
              "Bruce German y Moshe Rosenberg, del Departamento de Food Science and Technology de UC Davis, participaron en el Seminario “Leche y Salud Humana”, actividad  conjunta UC Davis Chile - Consorcio Lechero.",
            datePlace: "13 de diciembre, en Hotel Cumbres (Santiago).",
          },
          {
            id: "19",
            title:
              "Dr. Eduardo Silva, del Departamento de Biomedical Engineering de UC Davis, participó en la “NanoConference 2016: Biomedicine, Mining & Energy” -conferencia internacional organizada por CORFO y la Universidad Andrés Bello- y ofreció “Engineering new vascular nerwork with biomaterials”, charla organizada en colaboración con la Dirección de Desarrollo Tecnológico de la U. del Desarrollo (iCono UDD).",
            datePlace: "14 y 15 de diciembre, en Santiago.",
          },
        ],
      },
      {
        year: "2017",
        list: [
          {
            id: "20",
            title:
              'Pablo Zamora, Director Cientifico, habló sobre “UC Davis Chile y su propuesta de valor” a la delegación del curso de educación en liderazgo "Kansas Agricultural and Rural Leadership" KARL PROGRAM de la Kansas State University (Estados Unidos).',
            datePlace: "9 de marzo, Santiago.",
          },
          {
            id: "21",
            title:
              "Lawrence Kirkendall, profesor de la U. de Bergen (Noruega), dictó la charla “El fascinante mundo de los Escolítidos”",
            datePlace: "13 de marzo, en las oficinas de UC Davis Chile",
          },
          {
            id: "22",
            title:
              "Graham Fogg, del Center for Watershed Sciences de UC Davis, ofreció la charla “Sustainable Groundwater Management”. ",
            datePlace: "30 de marzo, en las oficinas de UC Davis Chile.",
          },
          {
            id: "23",
            title:
              "Pablo Zamora, Director cientifico; Álvaro Castro, Head of Research; Mark Battany, Extensionista especialista en viticultura del Sistema de Extensionismo de California; y Rodrigo Gallardo, profesor de la Escuela de Medicina Veterinaria de UC Davis, participaron con ponencias en la Feria Internacional de Tecnologías Agrícolas, IFT-Agro 2017.",
            datePlace: "6 y 7 de abril, Talca.",
          },
          {
            id: "24",
            title:
              "Freddy Boehmwald, Coordinador de Desarrollo de Bioproductos, encabezó con equipo de UC Davis Chile, realizó la presentación  a la comunidad Proyecto Colaborativo UTA - UC Davis Chile. Mientras que el Dr. Andrea Campisano ofreció la charla “Tales from the vineyard”.",
            datePlace: "12 de mayo, Universidad de Tarapacá (UTA), Arica.",
          },
          {
            id: "25",
            title:
              "Cleveland Justis, Director Instituto de Innovación de UC Davis, ofreció la charla “Science and Business for Social Benefit”.",
            datePlace:
              "17 de mayo en Corfo (Santiago) y 18 de mayo en la Facultad de Economía y Negocios de la U. de Talca (Talca).",
          },
          {
            id: "26",
            title:
              "Freddy Boehmwald, Coordinador de Desarrollo de Bioproductos, encabezó con equipo de UC Davis Chile, “Curso de Bioinformática”.",
            datePlace:
              "Mayo, en Facultad de Ciencias Agronómicas de la UTA, Arica.",
          },
          {
            id: "27",
            title: "Pablo Zamora, Director Asociado, en Creo en Chile.",
            datePlace: "15 de junio en Espacio Riesco",
          },
          {
            id: "28",
            title:
              "Carlos Flores, Coordinador Programas de Agronomía y Medio Ambiente “Adaptación al cambio climático y los recursos hídricos. Experiencia comparadas entre Chile y California”.",
            datePlace: "29 de junio, en la PUC.",
          },
          {
            id: "29",
            title:
              "Pablo Zamora, Director Asociado, dictó la charla “Innovation in Food: From research to innovative market products”.",
            datePlace:
              "16 de agosto, Pontificia Universidad Católica do Río Grande do Sul, Brasil",
          },
          {
            id: "30",
            title:
              "Climate Smart Agro Chile 2017; Jim Farrar, Director del Programa Estatal de Manejo Integrado de Plagas de División de Agricultura y Recursos Naturales de la U. de California; Alan Bennett, Director Ejecutivo de UC Davis Chile; y Carlos Flores, Coordinador Programas de Agronomía y Medio Ambiente",
            datePlace: "29 de agosto en Talca y 31 de agosto en Santiago.",
          },
          {
            id: "31",
            title:
              "Dr. Otis Littlefield, de Morrison Foerster (MOFO), una de las firmas de abogados más importantes en Propiedad Intelectual (PI) en Estados Unidos, ofreció charla “Buenas prácticas en patentamiento para la comercialización de tecnologías”.",
            datePlace: "4 de septiembre, en auditorium de Corfo (Santiago). ",
          },
          {
            id: "32",
            title:
              "Freddy Boehmwald, Coordinador de Desarrollo de Bioproductos, en International Food Safety Conference (IFSC).",
            datePlace:
              "6 de septiembre en Hotel Plaza El Bosque Manquehue    (Santiago).",
          },
          {
            id: "33",
            title:
              "Camille Kirke, Directora de Sustentabilidad de UC Davis, lideró el diálogo “Integrated Water Governance”, organizado con la American Academy el 5 de septiembre, en la U. de Talca, campus Santiago y el Tercer Encuentro Internacional Red Campus Sustentable (RCS), titulado “Sustentabilidad y Territorio”.",
            datePlace: "6 de septiembre, Talca.",
          },
          {
            id: "34",
            title:
              'Dario Cantu, profesor asistente del Department of Viticulture and Enology de UC Davis e investigador asociado a UC Davis Chile, ofreció el seminario “Leveraging plant and microbial genomics to study plant diseases in the field".',
            datePlace: "7 de septiembre, UNAB (Santiago).",
          },
          {
            id: "35",
            title:
              "Alan Bennett, Director Ejecutivo UC Davis Chile, en seminario “Propiedad Intelectual e Innovación en Agricultura y Sistemas Alimentarios”, organizado por la Misión Permanente de Chile ante la Organización Mundial de Propiedad Intelectual.",
            datePlace: "21 de septiembre, Ginebra (Suiza)",
          },
          {
            id: "36",
            title:
              "Carlos Flores, Coordinador de Agronomía y Medioambiente de UC Davis Chile, “Taller de Monitoreo de Calidad de Agua”.",
            datePlace: "26 de septiembre, Quillota",
          },
          {
            id: "37",
            title:
              "Pablo Zamora, Director Asociado UC Davis Chile, “The Innovation and Disruption Congress”, TIDCo.",
            datePlace:
              "5 de octubre, Escuela Superior Politécnica del Litoral, ESPOL, Guayaquil (Ecuador)",
          },
          {
            id: "38",
            title:
              "Álvaro Castro, Head of Research, en 6º Encuentro Ciencia, Tecnología y Empresa, organizado por Corfo.",
            datePlace: "5 de octubre, en edificio Telefónica",
          },
          {
            id: "39",
            title:
              "Carlos Flores, Coordinador de Agronomía y Medioambiente de UC Davis Chile, en Conversatorio Hidrotec: soluciones tecnológicas para la gestión hídrica y adaptación al cambio climático.",
            datePlace: "7 de noviembre, en CORFO",
          },
          {
            id: "40",
            title:
              "Charlas y capacitaciones del Doctor Leobardo Serrano, experto en fermentaciones con hongos y en escalamiento de estos procesos de la Universidad Nacional Autónoma de México (UNAM).",
            datePlace:
              "Lunes 13 y martes 14 en UC Davis Chile y entre el miércoles 15 y el viernes 17, en la Universidad de Tarapacá de Arica (UTA)",
          },
          {
            id: "41",
            title:
              "Hanan Eizenberg y Yaakov Goldwasser (former UC Davis postdoc), expertos en malezas de la Organización israelí para la Investigación Agrícola (ARO), “Experiencia israelita para el control de malezas”.",
            datePlace:
              "16 de noviembre en la Universidad de Talca y el martes 21 en el Ministerio de Agricultura (ODEPA). Agenda coordinada por UC Davis Chile.",
          },
          {
            id: "42",
            title:
              "Pablo Zamora, Director Asociado UC Davis Chile, 3er Encuentro Anual de Centros e Institutos Tecnológicos de Corfo.",
            datePlace: "27 de noviembre, CORFO",
          },
          {
            id: "43",
            title:
              "Carlos Flores, Coordinador de Agronomía y Medioambiente de UC Davis Chile, en seminario “Una mirada del sistema de riego chileno” para un comité de 15 personas del California Department of Agriculture.",
            datePlace: "27 de noviembre, Ministerio de Agricultura (ODEPA)",
          },
          {
            id: "44",
            title:
              "Catalina Pavez y Claudio Pavez, Asistentes de Investigación, con presentación de poster en XII Reunión Anual de Biología Vegetal. ",
            datePlace: "4 al 7 de diciembre, Villarrica",
          },
          {
            id: "45",
            title:
              "Dushyant Pathak, Vicerrector de Transferencia Tecnológica y de Relaciones Corporativas de UC Davis, con la charla “Translating innovative research into successful commercial impact”.",
            datePlace:
              "20 de diciembre, en cierre del Plan de Mejoramiento Institucional (PMI) de la UDD.",
          },
          {
            id: "46",
            title:
              "Cameron Carter, Vicerrector de Investigación de UC Davis, en charla “Frontiers in Neuroscience” para académicos, estudiantes de posgrado y médicos afiliados.",
            datePlace: "20 de diciembre en UDD.",
          },
        ],
      },
      {
        year: "2018",
        list: [
          {
            id: "47",
            title:
              "Paul Hastings, Profesor del Departmento de Psicología de UC Davis. Charla sobre “Procesos Biopsicosociales en el desarrollo prosocial” en actividad organizada por la UDD",
            datePlace:
              "jueves 11 de enero y charla informativa, en actividad organizada por UC Davis Chile, UC Davis y Fulbright Chile el jueves 18 de enero.",
          },
          {
            id: "48",
            title:
              "Jay Lund, Director de Center for Watershed Sciences de UC Davis, con la charla “Watershed management and riverine runoff in California”, Seminario “Land Sea Interactions in a Changing World: Science and Policy to Foster Conservation of Coastal Environments Services in Chile and California”, organizado por Centro de Cambio Global de la PUC. ",
            datePlace: "Miércoles 31 de enero",
          },
          {
            id: "49",
            title:
              "John Largier, Profesor del Departmento de Ciencias y Políticas Medioambientales y del Laboratorio Bodega de UC Davis, con la charla “The ocean needs water too”. Seminario “Land Sea Interactions in a Changing World: Science and Policy to Foster Conservation of Coastal Environments Services in Chile and California”, organizado por Centro de Cambio Global de la PUC.",
            datePlace: "Miércoles 31 de enero",
          },
          {
            id: "50",
            title:
              'Martin Hilbert, Associate Professor at UC Davis, California, Communication and Media, Social Policy and Sociocybernetics con la charla "Oportunidades y Desafíos de la Ciencia Social Computacional" en ExpoChileTEC, organizada por la Asociación de Empresas Chilenas de Tecnología',
            datePlace: "12 de junio de 2018.",
          },
          {
            id: "51",
            title:
              "Álvaro Castro, Head of Sciences UC Davis, Chile, panelista de la charla “Nuevas técnicas de mejora de cultivos, CRISPR y el marco regulatorio”",
            datePlace:
              "organizado por American Academy of Science and Technology, UC Davis Chile y UNAB.",
          },
          {
            id: "52",
            title:
              "Hub de Comercialización y Transferencia Tecnológica para las Américas, organizado por la OEA, UDD y UC Davis. “Ciencia colaborativa con foco en la demanda”, charla realizada por Daniela Sandoval, Partnerships Associate en UC Davis Chile, en el marco del Hub de Comercialización y Transferencia Tecnológica para las Américas, organizado por la OEA, UDD y UC Davis Chile. ",
            datePlace: "27 agosto al 27 septiembre.",
          },
          {
            id: "53",
            title: "Seminario Bioproductos",
            datePlace: "",
          },
          {
            id: "54",
            title:
              "Primera Cumbre Internacional de Bioinsumos, organizada en conjunto por UC Davis",
            datePlace: "Chile y MundoAgro -Septiembre.",
          },
          {
            id: "55",
            title:
              "“Descifrando el Viñedo Chileno” - Genomas de referencia del vi√±edo chileno: La ciencia tras la vid-. En el marco de la celebración del Día Nacional Del Vino. Organizan: UC Davis Chile en alianza con la Universidad Andrés Bello (UNAB) y las empresas Víña Concha y Toro y VSPT Wine Group. Participan: Alan Bennett, Dario Cantú, Alvaro Castro de UC Davis Chile. Ariel Orellana y Claudio Meneses, por parte de UNAB. Juan Cury, Gerente Agrícola y Abastecimiento de VSPT Wine Group y Gerard Casaubon, Director del CII de Viña Concha y Toro. ",
            datePlace: "4 septiembre",
          },
          {
            id: "56",
            title:
              "III USM Tech Innovation Summit, evento organizado por la Universidad Santa María (USM). Presentación de William “Bill” Tucker, Director Ejecutivo de Innovation Access de UC Davis.",
            datePlace: "20 noviembre",
          },
        ],
      },
      {
        year: "2019",
        list: [
          {
            id: "57",
            title:
              "Curso “Herramientas de extensión agrícola para asesores frutícolas de la Región de Valparaíso”. Iniciativa del Programa Estratégico Regional Fruticultura Sustentable, financiado por Corfo y el Gobierno Regional de Valparaíso, y ejecutado por UC Davis Chile. Dictaron el curso: especialistas de Extensión Cooperativa de la Universidad de California (UCCE): Mark Bell y Louise Ferguson.",
            datePlace: "5 febrero",
          },
          {
            id: "58",
            title:
              'Lanzamiento Chile Lagos Limpios – Panguipulli. Geoffrey Schladow, Director fundador de Tahoe Environmental Research Center (TERC) de UC Davis y parte del directorio de ChLL. Devin Middlebrook, Director de Sustentabilidad de la Agencia de Planificación regional del Lago Tahoe, y Lovell "Tu" Jarvis, Director Ejecutivo UCDC. Fernando Coz y Mauricio Cañoles. ',
            datePlace: "19 enero",
          },
          {
            id: "59",
            title:
              'charla " Translating innovative research into successful commercial impact" que realizaron en el Salón Rojo de CORFO. Dushyant Pathak, Vicerrector Asociado de Gestión Tecnológica y Relaciones Corporativas de UC Davis.',
            datePlace: "11 marzo",
          },
          {
            id: "60",
            title:
              "Taller Lineamientos para el desarrollo de la telemedicina y telesalud en Chile en contexto Bien Publico CORFO Telemedicina UDD, UdeC y UC Davis Chile.",
            datePlace: "29 marzo",
          },
          {
            id: "61",
            title:
              "Lanzamiento Bien Público “Central de Información y Modelamiento Hídrico”, CIMHi, inciativa fue impulsada por la Dirección de Aguas, DGA y cuenta con el financiamiento de Corfo. Mauricio Cañoles, General Manager, UCDC. ",
            datePlace: "",
          },
          {
            id: "62",
            title:
              "Taller Extension Agroinchalam Sistemas de conducción para uva de mesa - Monte Patria Coquimbo. Expositores: Martin Silva - Asesor Uva Mesa, Edwin Moore – Inchalam.",
            datePlace: "18 junio",
          },
          {
            id: "63",
            title:
              "Taller Extension Agroinchalam Sistemas de conducción para uva de mesa- Agricola San José Paine – Expositores: Martin Silva - Asesor Uva Mesa, Edwin Moore – Inchalam",
            datePlace: "27 junio",
          },
          {
            id: "64",
            title:
              "Workshop Universidad del Desarrollo en Docencia “Manejo de clima en el aula”- Margarita Jiménez, associate professor and director of teacher education at the School of Education",
            datePlace: "",
          },
          {
            id: "65",
            title:
              "UDD Tercer taller presencial “Hacia los lineamientos para el desarrollo de la telemedicina y telesalud en Chile” en contexto Bien Publico CORFO Telemedicina UDD, UdeC y UC Davis Chile.",
            datePlace: "2 agosto",
          },
          {
            id: "66",
            title:
              'Conferencia “Agricultura en un Mundo Cambiante”: Ciencia, tecnología, innovación y políticas públicas para revertir una crisis común que ya llegó. Presentan: Lovell "Tu" Jarvis, Presidente Consejo Chile California y Director Ejecutivo de UC Davis Chile y Daniel Sumner, Director of the University of California Agricultural Issues Center por videoconferencia Benjamin Houlton, director del Instituto del Medioambiente John Muir de UC Davis.',
            datePlace:
              "Organizan el Consejo Chile California (“Chile-California Council”), junto a UC Davis Chile, el Centro de la U. Católica de Cambio Global y el Instituto de Investigaciones Agropecuarias del Ministerio de Agricultura de Chile (INIA).",
          },
          {
            id: "67",
            title:
              "USM : III International Conference on Agro BigData and Decision Support Systems in Agriculture",
            datePlace: "25 al 27 septiembre",
          },
          {
            id: "68",
            title:
              "12 Americas Competitiveness Exchange (ACE) Organizado por OEA y UDD apoyado por UC Davis Chile y CORFO. Presentaciones de Camila Saavedra y Mauricio Cañoles de UCDC y de Isabel Moene de VSPT",
            datePlace: "6 al 10 de octubre",
          },
          {
            id: "69",
            title:
              "Conversatorio con Allan Fulton en UCDC. Extensionista en riego del CE California, junto a representantes de INIA, Pontificia Universidad Católica de Chile, Fruticultura Sustentable y Netafim Chile sobre las oportunidades y desafíos de Chile en la gestión del riego en condiciones de restricción hídrica.",
            datePlace: "22 noviembre",
          },
          {
            id: "70",
            title:
              "Día de Campo con Chile Prunes y Allan Fulton. Dia de campo en la region de O'Higgins. Andrés Olivos de PRUNOVA presenta el estado actual de las tecnologías de riego de ciruelo en Chile Prunes from Chile. ",
            datePlace: "23 noviembre",
          },
          {
            id: "71",
            title:
              "Taller Extension Agroinchalam sistema de conduccion en Cerezos – Osorno",
            datePlace: "22 noviembre. Presenta Marlen Araya, PUC",
          },
          {
            id: "72",
            title:
              "Taller Extension Agroinchalam sistema de conduccion en Cerezos – Angol",
            datePlace: "28 noviembre. Presenta Marlen Araya, PUC",
          },
          {
            id: "73",
            title:
              "Congreso Internacional Telemedicina UDD – en contexto Bien Publico CORFO Telemedicina UDD, UdeC y UC Davis Chile",
            datePlace: "6 diciembre. Concepción. ",
          },
        ],
      },
      {
        year: "2020",
        list: [
          {
            id: "74",
            title:
              "PMA Talks,	participación como Expositores. Olivia Valdés y Leticia Rojas, UC Davis Chile, Seminario online",
            datePlace: "17-06-20",
          },
          {
            id: "75",
            title:
              "ISSST Virtual Sessions. participación como expositores. Olivia Valdés, UC Davis Chile",
            datePlace: "Seminario online",
          },
          {
            id: "76",
            title:
              'Webinars: Establecimiento de vides y avances en la prevención y manejo de las enfermedades de la madera,	participación como co organizador, "Andrew Walker, UC Davis, Kendra Baumgartner, UC Davis"',
            datePlace: "Webinar, 01-07-20",
          },
          {
            id: "77",
            title:
              "Webinars: Establecimiento de vides y avances en la prevención y manejo de las enfermedades de la madera, participación como co organizador, Davis Gramaje, del Instituto de Ciencias de la Vid y el Vino",
            datePlace: "Webinar, 08-07-20",
          },
          {
            id: "78",
            title:
              "Presentación Estudio Economía Circular, participación como expositor,Olivia Valdés, UC Davis Chile, Presentación Online",
            datePlace: "21-07-20",
          },
          {
            id: "79",
            title:
              "Webinars: Establecimiento de vides y avances en la prevención y manejo de las enfermedades de la madera, participación como co organizador. José Ramón Urbez-Torres",
            datePlace: "Webinar, 24-07-20",
          },
          {
            id: "80",
            title:
              "Encuentro AmCham, participación como expositor. Olivia Valdés, UC Davis Chile Encuentro online",
            datePlace: "01-08-20",
          },
          {
            id: "81",
            title:
              'La problemática de Orobanche en tomate industrial: experiencias de Israel y California", participación como organizador. "Brad Hanson, UC Davis Alejandra Acuña, UC Davis Chile Yaakov Goldwasser "',
            datePlace: "Webinar, 04-08-20",
          },
          {
            id: "82",
            title:
              "El investigador emprededor, participación como expositor. Patricia Anguita, UC Davis Chile. Seminario online",
            datePlace: "05-08-20",
          },
          {
            id: "83",
            title:
              "El investigador emprededor, participación como expositor. Patricia Anguita, UC Davis Chile. Seminario online",
            datePlace: "06-08-20",
          },
          {
            id: "84",
            title:
              "UC Davis Global Conversation Series, participación como expositor. Ángela Delorenzo, Fundación Chile Lagos Limpios; Olga Barbosa, Head of the Regional Ministerial Secretariat for Science, Technology, Knowledge and Innovation for the South Macro Zone (SEREMI); Geoff Schladow, Director of the Tahoe Environmental Research Center UC Davis; Sebastian Vicuña, Director of the Center for Global Change; Lovell “Tu” Jarvis, Executive Director of the UC Davis Chile, 	Conversation Series",
            datePlace: "24-08-20",
          },
          {
            id: "85",
            title:
              "Información y modelación en cuencas hidrográficas, experiencia en California y el caso del Aconcagua, Chile, participación como organizador, Samuel Sandoval, UC Davis; Mauricio Cañoles, UC Davis Chile; Rodrigo Riveros , Junta vigilancia aconcagua; Oscar Cristi, Director Nacional DGA; Juan Fernando Acuña, Director Regional Corfo Valparaíso",
            datePlace: "Webinar, 24-08-20",
          },
          {
            id: "86",
            title:
              "Sesión en vivo: Potencial productivo y rentabilidad, participación como organizador, Gabino Reginato, académico Universidad de Chile; Cristián Valdés, asesor técnico de frutales. Sesión en vivo módulo I Ciruelo europeo",
            datePlace: "26-08-20",
          },
          {
            id: "87",
            title:
              'Soluciones para la Pérdida y Desperdicio de Alimentos, participación como organizador. Edward Spang, UC Davis; Mauricio Canoles, UC Davis Chile; Cristian Muñoz, hortofruticola; Graciela Urrutia, Transforma Alimentos; Karin Albornoz, UdeC; Stefanie Pope, Walmart"',
            datePlace: "Extension Talk, 27-08-20",
          },
          {
            id: "88",
            title:
              "Manejo del oídio en California, participación como organizador, Gabriel Torres, PhD. Viticulture Farm Advisor, University of California, Davis",
            datePlace: "Extension Talk, 03-09-20",
          },
          {
            id: "89",
            title:
              "Vitivinicultura 4.0: Aplicaciones Prácticas, participación como organizador. Kaan Kurtural, UC Davis; Ricardo Rodriguez Larrain, VSPT; Stanley Best, INIA; Alejandra Acuna, UC Davis Chile; Mauricio Canoles, UC Davis Chile.",
            datePlace: "Extension Talk, 09-09-20",
          },
          {
            id: "90",
            title:
              "Manejo de riego en frutales, Irrigation management: don´t ask me, ask the tree, participación como organizador. Kenneth Shackel, UC Davis; Samuel Barros, Andrés Olivos",
            datePlace: "Extension Talk, 23-09-20",
          },
          {
            id: "91",
            title:
              'Sesión en vivo: Sistemas de riego eficientes, participación como organizador."Blake Sanden, UC ANR; Alejandro Antúnez; Rosario Larraín. Sesión en vivo módulo II Ciruelo europeo',
            datePlace: "24-09-20",
          },
          {
            id: "92",
            title:
              "Expo Chile Agrícola, participación como expositor. Olivia Valdés, UC Davis Chile",
            datePlace: "Feria online, 29-09-20",
          },
          {
            id: "93",
            title:
              "Expo Chile Agrícola, participación como expositor. Leticia Rojas, UC Davis Chile",
            datePlace: "Feria online, 30-09-20",
          },
          {
            id: "94",
            title:
              "Expo Chile Agrícola, participación como expositor. Lovell Jarvis, UC Davis Chile; Mauricio Cañoles, UC Davis Chile.",
            datePlace: "Feria online, 30-09-20",
          },
          {
            id: "95",
            title:
              "Tips para el conocimiento científico, la innovación es hoy, participación como expositor. Patricia Anguita, UC Davis Chile.",
            datePlace: "Seminario online, 21-10-20",
          },
          {
            id: "96",
            title:
              "Riego de vides para vino, participación como organizador.	Larry Williams, UC Davis; Samuel Barros",
            datePlace: "Extension Talk, 28-10-29",
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
.timeline {
  line-height: 1.4em;
  list-style: none;
  margin: 0;
  padding: 0;
  width: 100%;
  h1,
  h2,
  h3,
  h4,
  h5,
  h6 {
    line-height: inherit;
  }
}

/*----- TIMELINE ITEM -----*/

.timeline-item {
  padding-left: 40px;
  position: relative;
  &:last-child {
    padding-bottom: 0;
  }
}

/*----- TIMELINE INFO -----*/

.timeline-info {
  font-size: 12px;
  font-weight: 700;
  letter-spacing: 2px;
  margin: 0 0 0.5em 0;
  text-transform: uppercase;
  color: $blue;
}
/*----- TIMELINE MARKER -----*/

.timeline-marker {
  position: absolute;
  top: 0;
  bottom: 0;
  left: 0;
  width: 15px;
  &:before {
    background: $gold;
    border: 3px solid transparent;
    border-radius: 100%;
    content: "";
    display: block;
    height: 15px;
    position: absolute;
    top: 4px;
    left: 0;
    width: 15px;
    transition: background 0.3s ease-in-out, border 0.3s ease-in-out;
  }
  &:after {
    content: "";
    width: 3px;
    background: #ccd5db;
    display: block;
    position: absolute;
    top: 24px;
    bottom: 0;
    left: 6px;
  }
  .timeline-item:last-child &:after {
    content: none;
  }
}
.timeline-item:not(.period):hover .timeline-marker:before {
  background: transparent;
  border: 3px solid $gold;
}

/*----- TIMELINE CONTENT -----*/

.timeline-content {
  padding-bottom: 40px;
  p:last-child {
    margin-bottom: 0;
  }
}

/*----- TIMELINE PERIOD -----*/

.period {
  padding: 0;
  .timeline-info {
    display: none;
  }
  .timeline-marker {
    &:before {
      background: transparent;
      content: "";
      width: 15px;
      height: auto;
      border: none;
      border-radius: 0;
      top: 0;
      bottom: 30px;
      position: absolute;
      border-top: 3px solid #ccd5db;
      border-bottom: 3px solid #ccd5db;
    }
    &:after {
      content: "";
      height: 32px;
      top: auto;
    }
  }
  .timeline-content {
    padding: 40px 0 70px;
  }
  .timeline-title {
    margin: 0;
    font-size: 35px;
  }
}

/*----------------------------------------------
        MOD: TIMELINE SPLIT
    ----------------------------------------------*/

.timeline-split {
  @media (min-width: 768px) {
    .timeline {
      display: table;
    }
    .timeline-item {
      display: table-row;
      padding: 0;
    }
    .timeline-info,
    .timeline-marker,
    .timeline-content,
    .period .timeline-info {
      display: table-cell;
      vertical-align: top;
    }
    .timeline-marker {
      position: relative;
    }
    .timeline-content {
      padding-left: 30px;
    }
    .timeline-info {
      padding-right: 30px;
    }
    .period .timeline-title {
      position: relative;
      left: -45px;
    }
  }
}

/*----------------------------------------------
        MOD: TIMELINE CENTERED
    ----------------------------------------------*/

.timeline-centered {
  @extend .timeline-split;
  @media (min-width: 992px) {
    &,
    .timeline-item,
    .timeline-info,
    .timeline-marker,
    .timeline-content {
      display: block;
      margin: 0;
      padding: 0;
    }
    .timeline-item {
      padding-bottom: 40px;
      overflow: hidden;
    }
    .timeline-marker {
      position: absolute;
      left: 50%;
      margin-left: -7.5px;
    }
    .timeline-info,
    .timeline-content {
      width: 50%;
    }
    > .timeline-item:nth-child(odd) .timeline-info {
      float: left;
      text-align: right;
      padding-right: 30px;
    }
    > .timeline-item:nth-child(odd) .timeline-content {
      float: right;
      text-align: left;
      padding-left: 30px;
    }
    > .timeline-item:nth-child(even) .timeline-info {
      float: right;
      text-align: left;
      padding-left: 30px;
    }
    > .timeline-item:nth-child(even) .timeline-content {
      float: left;
      text-align: right;
      padding-right: 30px;
    }
    > .timeline-item.period .timeline-content {
      float: none;
      padding: 0;
      width: 100%;
      text-align: center;
    }
    .timeline-item.period {
      padding: 40px 0 80px;
    }
    .period .timeline-marker:after {
      height: 30px;
      bottom: 0;
      top: auto;
    }
    .period .timeline-title {
      left: auto;
    }
  }
}

/*----------------------------------------------
        MOD: MARKER OUTLINE
    ----------------------------------------------*/

.marker-outline {
  .timeline-marker {
    &:before {
      background: transparent;
      border-color: $gold;
    }
  }
  .timeline-item:hover .timeline-marker:before {
    background: $gold;
  }
}
</style>