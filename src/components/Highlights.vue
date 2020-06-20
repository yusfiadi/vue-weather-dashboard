<template>
  <div class="custom-content-card content-card card">
    <div class="card-body pb-0">
      <div class="content-header h4 text-center pt-2 pb-3">Highlights</div>
      <div class="row">
        <UVIndex :uvIndex="uvIndex" />
        <WindStatus :windStatus="windStatus" />
        <Visibility :visibility="visibility" />
      </div>
    </div>
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