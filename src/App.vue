<script setup>
import { ref } from 'vue'
import MarsMap from './components/MarsMap.vue'
const map = ref(null)
</script>

<template>
  <div>
    <MarsMap ref="map" />
  </div>
</template>