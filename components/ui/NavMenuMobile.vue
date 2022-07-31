<template>
  <div>
    <ul class="links">
      <li><NuxtLink to="/our-company">Our Company</NuxtLink></li>
      <li><NuxtLink to="/locations">Locations</NuxtLink></li>
      <li><NuxtLink to="/contact">Contact</NuxtLink></li>
    </ul>
  </div>
</template>

<style lang="scss" scoped>
div {
  background: rgba(#000000, 0.5);
  height: 100vh;
  width: 100vw;
  position: fixed;
  top: 96px;
  left: 0;
  z-index: 2;
  color: $primary-white;
  font-size: 24px;

  ul {
    background: $primary-black;
    height: 235px;
    padding-left: 24px;
    padding-top: 50px;

    li {
      margin-bottom: 35px;

      a {
        color: $primary-white;
      }
    }

  }
}
</style>
