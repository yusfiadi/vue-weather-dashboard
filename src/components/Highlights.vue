<template>
  <div id="highlights">
    <UVIndex :uvIndex="uvIndex" />
    <WindStatus :windStatus="windStatus" />
    <Visibility :visibility="visibility" />
  </div>
</template>

<script>
import UVIndex from "./UVIndex";
import Visibility from "./Visibility";
import WindStatus from "./WindStatus";

export default {
  components: {
    UVIndex,
    Visibility,
    WindStatus
  },
  props: {
    highlights: {
      required: true,
      type: Object
    }
  },
  data() {
    return {
      uvIndex: this.highlights.uvIndex,
      windStatus: this.highlights.windStatus,
      visibility: this.highlights.visibility
    };
  }
};
</script>

<style>
</style>