
<template>
  <section>
    <GoogleMap
      :api-key="MyMapsApiKey"
      style="width: 100%; height: 500px; margin: 0 auto"
      :center="center"
      :zoom="15"
      :styles="mapStyles"
      :fullscreenControl="false"
      :panControl="false"
      :zoomControl="false"
      :mapTypeControl="false"
      :scaleControl="false"
      :streetViewControl="false"
      :overviewMapControl="false"
    >
      <Marker :options="{ position: center }" />
    </GoogleMap>
  </section>
</template>

<style lang="scss" scoped>
section {
  margin: 0 auto;
  max-width: 1440px;
  widows: 100%;
  height: 500px;
}
@import "@/scss/mixin";
GoogleMap {
  @include for-tablet-landscape {
    width: 1110px;
  }
}
</style>

<script>
import mapStyles from "/Front end/Final-beetroot-project/src/components/mapStyles.json";
import { MyMapsApiKey } from "/Front end/Final-beetroot-project/src/config.js";
import { defineComponent } from "vue";
import { GoogleMap, Marker } from "vue3-google-map";

export default defineComponent({
  name: "Mapsect",
  components: { GoogleMap, Marker },
  data() {
    return {
      MyMapsApiKey,
      center: { lat: 40.689247, lng: -74.044502 },
      mapStyles,
    };
  },
});
</script>