<template>
  <div id="visibility">
    <p>Visibility: {{ visibility }}</p>
  </div>
</template>

<script>
export default {
  props: {
    visibility: {
      type: String,
      required: true
    }
  }
};
</script>

<style>
</style>