<template>
  <div id="tempvarchart">
    <p>Temperature Information:</p>
    {{ tempVar }}
  </div>
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