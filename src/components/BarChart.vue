<script setup lang="ts">
import { Chart, type ChartItem } from "chart.js/auto";
import { ref, onMounted } from "vue";

const chartCanvas = ref<HTMLCanvasElement | null>(null); // Using ref for the canvas element

onMounted(() => {
  if (chartCanvas.value) {
    const ctx = chartCanvas.value.getContext("2d") as ChartItem; // Get the 2D rendering context

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
            barThickness: 10, // Adjust the bar thickness (in pixels)
            maxBarThickness: 50,
          },
        ],
      },
      options: {
        animation: {
          duration: 1500, // Duration of the filling up animation
          easing: "easeInQuad",
        },
        scales: {
          x: {
            grid: {
              display: false, // Disable grid lines on the x-axis
            },
            border: {
              display: false, // Remove the x-axis line
            },
          },
          y: {
            beginAtZero: true,
            ticks: {
              stepSize: 100,
            },
            grid: {
              display: false, // Disable grid lines on the y-axis
            },
            border: {
              display: false, // Remove the y-axis line
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
    <!-- Using the ref here -->
  </div>
</template>

<style scoped>
#bar-chart {
  width: 100%;
}
</style>
