<template>
  <div>
    <h1>Locations</h1>
    <div id="map-wrap" style="height: 100%">
      <client-only>
        <l-map :zoom=15 :center="[43.6350219,-79.4012992]">
          <l-tile-layer url="http://{s}.tile.osm.org/{z}/{x}/{y}.png"></l-tile-layer>
          <l-marker :lat-lng="[43.6350219,-79.4012992]"></l-marker>
        </l-map>
      </client-only>
    </div>
  </div>
</template>

<style lang="scss" scoped>
// Page - Coming Soon (Development Testing)
div {
  min-height: 150vh;
  text-align: center;
}
</style>
