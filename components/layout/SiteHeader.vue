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

      document.querySelector('html').classList.add("mobile-nav-prevent-scroll");
      document.querySelector('body').classList.add("mobile-nav-prevent-scroll");
    },
    closeMobileNav() {
      this.showMobileMenu = false;
      this.navMenuOpen = false

      document.querySelector('html').classList.remove("mobile-nav-prevent-scroll");
      document.querySelector('body').classList.remove("mobile-nav-prevent-scroll");
    }
  }
}
</script>

<style lang="scss" scoped>
  header {
    margin: 0 auto;
  }
</style>
