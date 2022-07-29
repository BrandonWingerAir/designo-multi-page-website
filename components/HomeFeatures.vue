<template>
  <section>
    <div>
      <img class="background-img" src="~/static/assets/shared/desktop/bg-pattern-small-circle.svg">
      <img src="~/static/assets/home/desktop/illustration-passionate.svg">
      <div>
        <h3>Passionate</h3>
        <p>
          Each project starts with an in-depth brand research to ensure we only create products that serve a purpose. We merge art, design, and technology into exciting new solutions.
        </p>
      </div>
    </div>
    <div>
      <img class="background-img" src="~/static/assets/shared/desktop/bg-pattern-small-circle.svg">
      <img src="~/static/assets/home/desktop/illustration-resourceful.svg">
      <div>
        <h3>Resourceful</h3>
        <p>
          Everything that we do has a strategic purpose. We use an agile approach in all of our projects and value customer collaboration. It guarantees superior results that fulfill our clients’ needs.
        </p>
      </div>
    </div>
    <div>
      <img class="background-img" src="~/static/assets/shared/desktop/bg-pattern-small-circle.svg">
      <img src="~/static/assets/home/desktop/illustration-friendly.svg">
      <div>
        <h3>Friendly</h3>
        <p>
          We are a group of enthusiastic folks who know how to put people first. Our success depends on our customers, and we strive to give them the best experience a company can provide.
        </p>
      </div>
    </div>
  </section>
</template>

<style lang="scss" scoped>
section {
  display: grid;
  grid: 100% / 1fr 1fr 1fr;
  text-align: center;
  position: relative;

  div {
    padding: 0 12px;

    .background-img {
      position: absolute;
    }

    &:nth-of-type(2) {
      .background-img {
        transform: rotate(-90deg);
      }
    }

    &:last-of-type {
      .background-img {
        transform: rotate(90deg);
      }
    }

    img {
      position: relative;
      margin-bottom: 50px;
    }

    h3 {
      font-size: $heading-3-size;
      line-height: $heading-3-height;
      letter-spacing: $heading-3-spacing;
      font-weight: 500;
      text-transform: uppercase;
      margin-bottom: 50px;
    }

    p {
      @include body-text;
    }
  }

  @media only screen and (max-width: $tablet-max-width-landscape) {
    grid-template-columns: 1fr;

    div {
      display: flex;
      align-items: center;
      padding: 0;

      div {
        display: block;
        text-align: left;
        margin-left: 50px;

        h3 {
          margin-top: -48px;
          margin-bottom: 24px;
        }

        p {
          width: 440px;
        }
      }
    }
  }
}
</style>
