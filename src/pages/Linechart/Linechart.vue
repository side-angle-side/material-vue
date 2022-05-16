<template xmlns:div="http://www.w3.org/1999/html">
  <v-container fluid class="notification-page">
    <h1 class="page-title mt-10 mb-9">Notifications</h1>
    <v-card width="100%" class="d-flex flex-row mx-3" height="500px"
      ><v-row no-gutters>
        <v-chart
          class="chart"
          :option="option"
          height="500px"
        ></v-chart> </v-row
    ></v-card>
    <v-card width="100%" class="d-flex flex-row mx-3"></v-card>
  </v-container>
</template>

<script>
export default {
  name: "Linechart",
  data() {
    return {
      option: {
        title: {
          text: "ECharts 入门示例",
        },
        tooltip: {},
        xAxis: {
          data: ["衬衫", "羊毛衫", "雪纺衫", "裤子", "高跟鞋", "袜子"],
        },
        yAxis: {},
        series: [
          {
            name: "销量",
            type: "bar",
            data: [5, 20, 36, 10, 10, 20],
          },
        ],
      },
    };
  },
};
</script>

<style src="./Linechart.scss" lang="scss"></style>
