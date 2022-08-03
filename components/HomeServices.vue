<template>
  <section>
    <div>
      <div>
        <h2>Web Design</h2>
        <NuxtLink to="/our-company">
          View Projects <img src="~/static/assets/shared/desktop/icon-right-arrow.svg" alt="">
        </NuxtLink>
      </div>
    </div>
    <div>
      <div>
        <h2>App Design</h2>
        <NuxtLink to="/our-company">
          View Projects <img src="~/static/assets/shared/desktop/icon-right-arrow.svg" alt="">
        </NuxtLink>
      </div>
    </div>
    <div>
      <div>
        <h2>Graphic Design</h2>
        <NuxtLink to="/our-company">
          View Projects <img src="~/static/assets/shared/desktop/icon-right-arrow.svg" alt="">
        </NuxtLink>
      </div>
    </div>
  </section>
</template>

<style lang="scss" scoped>
section {
  display: grid;
  grid-template-columns: 1fr 1fr;
  column-gap: 30px;
  row-gap: 24px;
  height: 640px;

  > div {
    display: flex;
    justify-content: center;
    align-items: center;
    border-radius: 20px;

    &:hover {
      cursor: pointer;
    }

    &:first-of-type {
      @include home-web-design-card;

      &:hover {
        background: $img-web-design-lg-hover;
      }
    }

    &:nth-of-type(2) {
      @include home-app-design-card;

      &:hover {
        background: $img-app-design-hover;
      }
    }

    &:last-of-type {
      @include home-graphic-design-card;

      &:hover {
        background: $img-graphic-design-hover;
      }
    }

    div {
      text-align: center;
      color: $primary-white;
      text-transform: uppercase;
    }

    h2 {
      font-weight: 500;
      margin-bottom: 25px;
    }

    a {
      color: $primary-white;
      font-size: 15px;
      letter-spacing: 5px;
      width: 50px;

      img {
        margin-left: 10px;
      }
    }
  }

  @media only screen and (max-width: $tablet-max-width-landscape) {
    height: auto;
    grid-template-columns: 1fr;

    > div {
      height: 200px;

      &:first-of-type {
        @include home-web-design-card-tablet;

        &:hover {
          background: $img-web-design-tablet-hover;
        }
      }

      &:nth-of-type(2) {
        @include home-app-design-card-tablet;

        &:hover {
          background: $img-app-design-tablet-hover;
        }
      }

      &:last-of-type {
        @include home-graphic-design-card-tablet;

        &:hover {
          background: $img-graphic-design-tablet-hover;
        }
      }
    }
  }

  @media only screen and (max-width: $phone-max-width) {
    > div {
      height: 250px;

      &:first-of-type {
        @include home-web-design-card-phone;

        &:hover {
          background: $img-web-design-phone-hover;
        }
      }

      &:nth-of-type(2) {
        @include home-app-design-card-phone;

        &:hover {
          background: $img-app-design-phone-hover;
        }
      }

      &:last-of-type {
        @include home-graphic-design-card-phone;

        &:hover {
          background: $img-graphic-design-phone-hover;
        }
      }

      h2 {
        font-size: 28px;
        margin-bottom: 5px;
      }

      a {
        letter-spacing: 6px;

        img {
          margin-left: 5px;
        }
      }
    }
  }
}
</style>
