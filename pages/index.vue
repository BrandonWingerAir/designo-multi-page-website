<template>
  <div>
      <main class="content-margin">
        <HomeHero/>
        <HomeServices class="content-margin-phone"/>
        <HomeFeatures class="content-margin-phone"/>
      </main>
      <div class="bg-img-bottom"></div>
  </div>
</template>

<style lang="scss" scoped>
main {
  position: relative;

  section {
    margin-bottom: 160px;
    z-index: 1;

    &:last-of-type {
      margin-bottom: 380px;
    }
  }
}

.bg-img-bottom {
  position: absolute;
  top: 1880px;
  left: 236px;
  height: 594px;
  width: 100%;
  background: url('~static/assets/shared/desktop/bg-pattern-leaf.svg') center no-repeat;
  transform: rotate(180deg);
}


@media only screen and (max-width: $tablet-max-width-landscape) {
  main > section {
    margin-bottom: 120px;

    &:last-of-type {
      margin-bottom: 330px;
    }
  }

  .bg-img-bottom {
    display: none;
  }
}

@media only screen and (max-width: $phone-max-width) {
  main > section:last-of-type {
    margin-bottom: 230px;
  }
}
</style>
