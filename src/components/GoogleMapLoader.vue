<template>
   <GmapMap
  :center="center"
  :zoom="15"
  style="width: 100%; height: 100%"
  >
  <GmapMarker
    :key="index"
    v-for="(m, index) in markers"
    :position="m.position"
    :clickable="true"
    :draggable="true"
    @click="center=m.position"
  />
</GmapMap>
</template>

<script>
export default {
   name: 'GoogleMapLoader',
   data(){
       return{
           center: {lat:37.803356510938045, lng:-122.47281976024624},
           markers:[
               {
                   position:{lat: 37.803356510938045, lng:-122.47281976024624}
                }
           ]
       }
   }
}
</script>

<style>

</style>