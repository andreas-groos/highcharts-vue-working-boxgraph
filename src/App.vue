<template>
  <div id="app">
    <img src="./assets/logo.png">
    <highcharts :options="chartOptions"></highcharts>

  </div>
</template>

<script>
import { Chart } from "highcharts-vue";

export default {
  name: "App",
  components: {
    highcharts: Chart
  },
  data() {
    return {
      chartOptions: {
        series: [
          {
            data: [1, 2, 3] // sample data
          }
        ]
      }
    };
  }
};
</script>

<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
