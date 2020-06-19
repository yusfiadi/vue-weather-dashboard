<template>
  <div id="app">
    <p>This component’s code is in {{ filename }}</p>
  </div>
</template>

<script>
export default {
  name: "app",
  data() {
    return {
      filename: "App.vue"
    };
  }
};
</script>

<style lang="scss">
</style>
