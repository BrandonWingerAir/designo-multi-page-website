<template>
  <nav>
    <NuxtLink to="/"><img class="logo" src="~/static/assets/shared/desktop/logo-dark.png"/></NuxtLink>

    <ul class="links">
      <li><NuxtLink to="/our-company">Our Company</NuxtLink></li>
      <li><NuxtLink to="/locations">Locations</NuxtLink></li>
      <li><NuxtLink to="/contact">Contact</NuxtLink></li>
    </ul>

    <img class="mobile-nav-btn" src="~/static/assets/shared/mobile/icon-hamburger.svg" alt=""/>
  </nav>
</template>

<style lang="scss" scoped>
  nav {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 64px 0;

    .logo {
      width: 202px;
      height: 27px;
    }

    div > a {
      display: flex;
    }

    .links {
      font-size: 14px;
      height: 27px;
      display: flex;
      align-items: flex-end;
      list-style: none;

      a {
        color: $secondary-dark-grey;
        text-transform: uppercase;
        font-weight: 400;
        letter-spacing: 2px;
        margin-left: 40px;

        &:hover {
          text-decoration: underline;
          text-decoration-color: #9e9e9e;
        }
      }
    }

    @media only screen and (max-width: $phone-max-width) {
      padding: 0;
      height: 96px;

      .logo {
        margin-left: 24px;
        margin-top: 7px;
      }

      .links {
        display: none;
      }

      .mobile-nav-btn {
        position: absolute;
        right: 24px;
      }
    }
  }
</style>
