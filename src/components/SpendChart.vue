<script>
import { Bar } from "vue-chartjs";

export default {
  name: "SpendChart",
  extends: Bar,
  data: () => ({
    chartdata: {
      labels: ["1. Fase Instalación", "2. Fase Operación"],
      datasets: [
        {
          label: "Partnership",
          backgroundColor: "#C6007E",
          stack: "Stack 0",
          data: [300, 627],
        },
        {
          label: "Transferencia y Extensión",
          backgroundColor: "#00C4B3",
          stack: "Stack 0",
          data: [215, 1298],
        },
        {
          label: "Investigación",
          backgroundColor: "#f095CD",
          stack: "Stack 0",
          data: [3404, 2524],
        },
        {
          label: "Administración",
          backgroundColor: "#FFBF00",
          stack: "Stack 0",
          data: [1879, 1783],
        },
      ],
    },
    options: {
      responsive: true,
      maintainAspectRatio: false,
      legend: {
        position: "bottom",
      },
      scales: {
        yAxes: [
          {
            scaleLabel: {
              display: true,
              labelString: "Millones de pesos",
            },
          },
        ],
      },
    },
  }),
  mounted() {
    this.renderChart(this.chartdata, this.options);
  },
};
</script>