<template>
  <div>
    <div class="bg-image">
      <SiteHeader/>
      <Nuxt/>
    </div>
    <FooterContact/>
    <SiteFooter/>
  </div>
</template>

<style lang="scss" scoped>
.bg-image {
  background: url('~static/assets/shared/desktop/bg-pattern-leaf.svg') left 281px no-repeat;

  @media only screen and (max-width: $tablet-max-width-landscape) {
    background: initial;
  }
}
</style>
