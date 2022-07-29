<template>
  <div class="section-container">
    <section class="content-margin">
      <div class="card-container">
        <div>
          <h2>
            Let’s talk about <br>
            your project
          </h2>
          <p>
            Ready to take it to the next level? Contact us today and find out how <br>
            our expertise can help your business grow.
          </p>
        </div>
      </div>
      <div class="card-container">
        <NuxtLink to="contact">
          <button class="btn-light">Get in touch</button>
        </NuxtLink>
      </div>
    </section>
  </div>
</template>

<style lang="scss" scoped>
.section-container {
  position: relative;
  display: flex;
  justify-content: center;

  section {
    background: url('~static/assets/shared/desktop/bg-pattern-call-to-action.svg') no-repeat 235px center $primary-peach;
    height: 292px;
    border-radius: 15px;
    color: $primary-white;
    display: grid;
    grid: 100% / 2fr 1fr;
    position: absolute;
    z-index: 1;
    top: -220px;

    .card-container {
      display: flex;
      align-items: center;
      padding: 0 95px;

      &:last-of-type {
        justify-content: right;
      }
    }

    h2 {
      font-weight: 500;
      margin-bottom: 15px;
    }

    p {
      font-weight: 300;
    }
  }

  @media only screen and (max-width: $tablet-max-width-landscape) {
    section {
      display: block;
      height: 350px;
      top: -265px;
      text-align: center;

      background-position: -30px center;

      .card-container {
        padding-top: 60px;

        div {
          width: 100%;

          h2 {
            line-height: 38px;
          }

          p {
            line-height: 24px;
          }
        }

        &:last-of-type {
          justify-content: center;
          padding-top: 35px;
        }
      }
    }
  }
}

</style>
