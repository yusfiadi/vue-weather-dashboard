<template>
  <div>{{ tempVar.tempToday }}</div>
</template>

<script>
export default {
  props: {
    tempVar: {
      required: true,
      type: Object
    }
  },
  data() {
    return {};
  }
};
</script>

<style>
</style>