<template>
  <section>
      <div class="location-card">
        <h2>Canada</h2>
        <h4>Designo Central Office</h4>
        <h4>3886 Wellington Street</h4>
        <h4>Toronto, Ontario M9C 3J5</h4>
      </div>
      <div id="map-wrap" style="height: 326px">
        <client-only>
          <l-map :zoom=15 :center="[43.6350219,-79.4012992]">
            <l-tile-layer url="http://{s}.tile.osm.org/{z}/{x}/{y}.png"></l-tile-layer>
            <l-marker :lat-lng="[43.6350219,-79.4012992]"></l-marker>
          </l-map>
        </client-only>
      </div>
  </section>
</template>

<style lang="scss" scoped>
section {
  min-height: 80vh;
  display: grid;
  grid-template-columns: 730px 350px;
  column-gap: 33px;

  .location-card {
    background: $card-lighter-peach;
  }

  > div {
    height: 326px;

    h4 {
      font-weight: normal;
    }

    h4:first-of-type {
      font-weight: bold;
    }
  }
}
</style>
