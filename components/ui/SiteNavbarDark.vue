<template>
  <nav>
    <NuxtLink to="/"><img src="/assets/shared/desktop/logo-dark.png"/></NuxtLink>

    <ul>
      <li><NuxtLink to="/our-company">Our Company</NuxtLink></li>
      <li><NuxtLink to="/locations">Locations</NuxtLink></li>
      <li><NuxtLink to="/contact">Contact</NuxtLink></li>
    </ul>
  </nav>
</template>

<style lang="scss" scoped>
  nav {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 64px 0;
  }

  img {
    width: 202px;
    height: 27px;
  }

  div > a {
    display: flex;
  }

  ul {
    font-size: 14px;
    height: 27px;
    display: flex;
    align-items: flex-end;
    list-style: none;

    a {
      color: $secondary-dark-grey;
      text-decoration: none;
      text-transform: uppercase;
      font-weight: 400;
      letter-spacing: 2px;
      margin-left: 40px;
    }
  }
</style>
