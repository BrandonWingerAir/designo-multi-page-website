<template>
  <nav>
    <NuxtLink to="/"><img src="~/static/assets/shared/desktop/logo-light.png"/></NuxtLink>

    <hr class="content-margin-phone"/>

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
    padding: 144px 0 45px;

    img {
      width: 202px;
      height: 27px;
    }

    hr {
      display: none;
    }

    ul {
      font-size: 14px;
      height: 27px;
      display: flex;
      align-items: flex-end;
      list-style: none;

      a {
        color: $primary-white;
        text-transform: uppercase;
        font-weight: 300;
        letter-spacing: 2px;
        margin-left: 40px;

        &:hover {
          text-decoration: underline;
          text-decoration-color: #9e9e9e;
        }
      }
    }

    @media only screen and (max-width: $tablet-max-width-landscape) {
      padding: 165px 0 45px;
    }

    @media only screen and (max-width: $phone-max-width) {
      display: block;
      text-align: center;
      padding: 250px 0 5px;

      hr {
        display: block;
        margin: 30px auto;
        border: none;
        height: 1px;
        background-color: #424242;
      }

      ul {
        display: block;
        height: 100%;

        li {
          margin-bottom: 30px;
        }

        a {
          margin-left: 0;
        }
      }
    }
  }
</style>
