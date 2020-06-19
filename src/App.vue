<template>
  <div id="app">
    <p>This component’s code is in {{ filename }}</p>
    <Content :weather-data="weatherData"></Content>
  </div>
</template>

<script>
import Content from "@/components/Content";
export default {
  name: "app",
  components: {
    Content
  },
  data() {
    return {
      filename: "App.vue",
      weatherData: {
        location: "California",
        temperature: {
          current: "35 C"
        },
        highlights: {
          uvindex: "3",
          windstatus: {
            speed: "20 km/h",
            direction: "N-E"
          },
          visibility: "12 km"
        }
      }
    };
  }
};
</script>

<style lang="scss">
</style>
