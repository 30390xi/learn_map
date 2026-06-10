<template>
    <div id="marsMap" class="map"></div>
</template>
<script setup>
import { onMounted } from 'vue'
onMounted(() => {
  const map = new mars3d.Map('marsMap', {
    scene: {
      center: {
        lat: 31.3288,
        lng: 105.753253,
        alt: 25000000,
        heading: 0,
        pitch: -90,
      },
    },
  });

  window.map = map;
});
</script>
<style scoped>
.map {
    width: 100vw;
    height: 100vh;
}
</style>