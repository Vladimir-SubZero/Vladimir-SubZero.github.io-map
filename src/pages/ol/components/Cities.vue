
<template>
    <div class="root">
        <div id="map" class="map"></div>
    </div>
</template>

<script setup lang="ts">
import { useMap } from '../compositionUtils/useOlMap.ts'

useMap()


</script>

<style lang="sass">
.root
    width: 100%
    height: 100%

.map 
    width: 100%
    height: calc(100vh - 60px)

.ol-zoom 
    display: flex
    flex-direction: column
    width: 25px
    height: auto
    position: absolute
    bottom: 20px
    right: 10px
    border: 1px solid #fcf
    border: none

.ol-zoom-in
    margin-bottom: 2px
    border-radius: 5px
.ol-zoom-out
    border-radius: 5px
.ol-rotate
    display: none

</style>