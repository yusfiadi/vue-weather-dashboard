<template>
  <div id="highlights">
    <p>Weather Highlights:</p>
    {{ highlights }}
    <UVIndex :uvindex="uvindex" />
    <WindStatus :windstatus="windstatus" />
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
      uvindex: this.highlights.uvindex,
      windstatus: this.highlights.windstatus,
      visibility: this.highlights.visibility
    };
  }
};
</script>

<style>
</style>