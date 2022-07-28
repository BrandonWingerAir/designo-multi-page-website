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
}
</style>
