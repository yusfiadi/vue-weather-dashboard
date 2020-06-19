<template>
  <div id="windstatus">
    <p>Wind Status:</p>
    <p>Speed — {{ windstatus.speed }}; Direction — {{ windstatus.direction }}</p>
  </div>
</template>

<script>
export default {
  props: {
    windstatus: {
      type: Object,
      required: true
    }
  }
};
</script>

<style>
</style>