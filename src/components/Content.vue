<template>
  <div id="pageContent">
    <p>This child components of Content.vue are:</p>
    <ul>
      <li v-for="child in childComponents" :key="child.id">{{ child }}</li>
    </ul>
    {{ weatherData }}
  </div>
</template>

<script>
export default {
  data() {
    return {
      childComponents: ["TempVarChart.vue", "Highlights.vue"]
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
