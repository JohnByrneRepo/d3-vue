<template>
  <div class="example">
    <BarChart
      class="chart"
      :data-set="data"
      :margin-left="40"
      :margin-top="40"
      :tick-count="5"
      :bar-padding="0.5"
    />
  </div>
</template>

<script>
import BarChart from "./components/BarChart.vue";

export default {
  name: "example",
  data() {
    return {
      data: [
        ["Test 1", 33],
        ["Test 2", 24],
        ["Test 3", 22],
        ["Test 4", 12],
        ["Test 5", 43],
        ["Test 6", 23],
        ["Test 7", 2],
        ["Test 8", 35]
      ]
    };
  },
  components: {
    BarChart
  }
};
</script>

<style scoped>
.chart {
  margin: 40px auto 0;
  display: block;
}
</style>
