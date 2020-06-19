<template>
  <div style="position: relative;">
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
    return {};
  },
  props: {
    tempVar: {
      required: true,
      type: Object
    },
    highlights: {
      type: Object,
      required: true
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
