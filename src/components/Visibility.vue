<template>
  <div>
    <p>Visibility: {{ visibility }}</p>
  </div>
</template>

<script>
export default {
  props: {
    visibility: {
      type: Number,
      required: true
    }
  },
  data() {
    return {};
  }
};
</script>

<style>
</style>