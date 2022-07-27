<template>
  <div>
      <main class="content-margin">
        <HomeHero/>
        <HomeServices/>
        <HomeFeatures/>
      </main>
      <div class="bg-img-bottom"></div>
  </div>
</template>

<style lang="scss" scoped>
main {
  position: relative;
}

.bg-img-bottom {
  position: absolute;
  top: 1880px;
  left: 236px;
  height: 594px;
  width: 100%;
  background: url('/assets/shared/desktop/bg-pattern-leaf.svg') center no-repeat;
  z-index: 0;
}

section {
  margin-bottom: 160px;
  z-index: 1;

  &:last-of-type {
    margin-bottom: 380px;
  }
}
</style>
