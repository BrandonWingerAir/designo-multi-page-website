<template>
  <section>
    <div>
      <div>
        <h2>Web Design</h2>
        <NuxtLink to="/our-company">
          View Projects <img src="/assets/shared/desktop/icon-right-arrow.svg" alt="">
        </NuxtLink>
      </div>
    </div>
    <div>
      <div>
        <h2>App Design</h2>
        <NuxtLink to="/our-company">
          View Projects <img src="/assets/shared/desktop/icon-right-arrow.svg" alt="">
        </NuxtLink>
      </div>
    </div>
    <div>
      <div>
        <h2>Graphic Design</h2>
        <NuxtLink to="/our-company">
          View Projects <img src="/assets/shared/desktop/icon-right-arrow.svg" alt="">
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

    &:first-of-type {
      grid-row: 1 / 3;
      background: $img-web-design-lg;
    }

    &:nth-of-type(2) {
      background: $img-app-design;
    }

    &:last-of-type {
      background: $img-graphic-design;
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

      > img {
        margin-left: 10px;
      }
    }
  }
}
</style>
