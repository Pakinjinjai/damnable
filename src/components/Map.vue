<script setup>
import { GoogleMap, Marker } from 'vue3-google-map'

const center1 = { lat: 10.708058008401881, lng: 99.31851661965551 }
const center2 = { lat: 10.724289286807188, lng: 99.37513730778062 }
const center3 = { lat: 10.773281127301155, lag: 99.39760320951709 }
</script>

<template>
  <GoogleMap
  api-key="AIzaSyBXQR8cx4NVv0YYbBAUZmarrBB6fcD2We8"
  style="width: 1200px; height: 1000px"
  :center="center2"
  :zoom="10"
  >
    <Marker :options="{ position: center1 }" />
    <Marker :options="{ position: center2 }" />
    <Marker :options="{ position: center3 }" />
  </GoogleMap>
</template>