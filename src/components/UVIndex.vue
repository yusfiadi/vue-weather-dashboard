<template>
  <div id="uvIndex">
    <p>UV Index: {{ uvIndex }}</p>
  </div>
</template>

<script>
export default {
  props: {
    uvIndex: {
      type: Number,
      required: true
    }
  }
};
</script>

<style>
</style>