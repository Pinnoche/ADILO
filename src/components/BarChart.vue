<script setup lang="ts">
import { Chart, type ChartItem } from "chart.js/auto";
import { ref, onMounted } from "vue";

const chartCanvas = ref<HTMLCanvasElement | null>(null); 

onMounted(() => {
  if (chartCanvas.value) {
    const ctx = chartCanvas.value.getContext("2d") as ChartItem; 

    new Chart(ctx, {
      type: "bar",
      data: {
        labels: [
          "Jan",
          "Feb",
          "Mar",
          "Apr",
          "May",
          "Jun",
          "Jul",
          "Aug",
          "Sep",
          "Oct",
          "Nov",
          "Dec",
        ],
        datasets: [
          {
            label: "",
            data: [100, 120, 120, 220, 250, 180, 200, 100, 300, 350, 380, 400],
            borderWidth: 0,
            borderRadius: 32,
            backgroundColor: "#1B59F8CC",
            barThickness: 10,
            maxBarThickness: 50,
          },
        ],
      },
      options: {
        animation: {
          duration: 1500, 
          easing: "easeInQuad",
        },
        scales: {
          x: {
            grid: {
              display: false, 
            },
            border: {
              display: false,
            },
          },
          y: {
            beginAtZero: true,
            ticks: {
              stepSize: 100,
            },
            grid: {
              display: false,
            },
            border: {
              display: false,
            },
          },
        },
        plugins: {
          legend: {
            display: false,
          },
        },
      },
    });
  }
});
</script>

<template>
  <div id="bar-chart">
    <canvas ref="chartCanvas" id="myChart" width="500" height="300"></canvas>
  </div>
</template>

<style scoped>
#bar-chart {
  width: 100%;
}
</style>
