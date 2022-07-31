<template>
  <header class="content-margin">
    <!-- <SiteNavbarDark :showMobileMenu="showMobileMenu" @showMobileMenu="showMobileMenu = true"/> -->
    <SiteNavbarDark :navMenuOpen="navMenuOpen" @showMobileMenu="showMobileMenu = true; navMenuOpen = true" @closeMobileMenu="showMobileMenu = false; navMenuOpen = false"/>
    <NavMenuMobile v-show="showMobileMenu"/>
  </header>
</template>

<script>
export default {
  data () {
    return {
      showMobileMenu: false,
      navMenuOpen: false
    }
  }
}
</script>

<style lang="scss" scoped>
  header {
    margin: 0 auto;
  }
</style>
