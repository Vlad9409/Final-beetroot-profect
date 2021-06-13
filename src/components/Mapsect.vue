
<template>
  <GoogleMap
    :api-key="MyMapsApiKey"
    style="width: 1440px; height: 500px; margin: 0 auto"
    :center="center"
    :zoom="15"
    :styles="mapStyles"
  >
    <Marker :options="{ position: center }" />
  </GoogleMap>
</template>

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