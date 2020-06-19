<template>
  <div id="pageContent">
    <p>This child components of Content.vue are:</p>
    <ul>
      <li v-for="child in childComponents" :key="child.id">{{ child }}</li>
    </ul>
    {{ weatherData }}
    <TempVarChart :tempVar="tempVar" />
    <TodayHighlights :highlights="highlights" />
  </div>
</template>

<script>
import TempVarChart from "./TempVarChart";
import Highlights from "./Highlights";
export default {
  components: {
    TempVarChart,
    TodayHighlights: Highlights
  },
  data() {
    return {
      childComponents: ["TempVarChart.vue", "Highlights.vue"],
      tempVar: this.weatherData.temperature,
      highlights: this.weatherData.highlights
    };
  },
  props: {
    weatherData: {
      required: true,
      type: Object
    }
  },
  methods: {},
  computed: {}
};
</script>

<style scoped>
#pagecontent {
  border: 1px solid black;
  padding: 2px;
}
</style>
