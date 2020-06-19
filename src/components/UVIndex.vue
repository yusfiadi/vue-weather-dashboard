<template>
  <div id="uvindex">
    <p>UV Index: {{ uvindex }}</p>
  </div>
</template>

<script>
export default {
  props: {
    uvindex: {
      type: String,
      required: true
    }
  }
};
</script>

<style>
</style>