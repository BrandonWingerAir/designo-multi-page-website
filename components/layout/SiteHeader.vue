<template>
  <header class="content-margin">
    <SiteNavbarDark :navMenuOpen="navMenuOpen" @showMobileMenu="openMobileNav" @closeMobileMenu="closeMobileNav"/>
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
  },
  methods: {
    openMobileNav() {
      this.showMobileMenu = true;
      this.navMenuOpen = true;
      document.querySelector("html").style.overflowY = "hidden";
    },
    closeMobileNav() {
      this.showMobileMenu = false;
      this.navMenuOpen = false
      document.querySelector("html").style.overflowY = "initial";
    }
  }
}
</script>

<style lang="scss" scoped>
  header {
    margin: 0 auto;
  }
</style>
