<template>
  <div>
    <p>Wind Speed — {{ windSpeed }}</p>
    <p>Wind Direction — {{ derivedWindDirection }}, or {{ windDirection }} degree clockwise with respect to true N as 0 degree.</p>
  </div>
</template>

<script>
export default {
  props: {
    windStatus: {
      type: Object,
      required: true
    }
  },
  data() {
    return {
      windSpeed: this.windStatus.windSpeed,
      derivedWindDirection: this.windStatus.derivedWindDirection,
      windDirection: this.windStatus.windDirection
    };
  }
};
</script>

<style>
</style>