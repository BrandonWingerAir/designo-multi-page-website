<template>
  <section>
    <img src="~/static/assets/home/desktop/bg-pattern-hero-home.svg"/>
    <div class="bg-img-container">
      <img src="~/static/assets/home/desktop/image-hero-phone.png">
    </div>
    <div class="text-container">
      <h1>Award-winning custom designs and digital branding solutions</h1>
      <p>
        With over 10 years in the industry, we are experienced in creating fully responsive websites, app design, and engaging brand experiences. Find out more about our services.
      </p>
      <NuxtLink to="our-company">
        <button class="btn-light">Learn more</button>
      </NuxtLink>
    </div>
  </section>
</template>

<style lang="scss" scoped>
  section {
    position: relative;
    height: 640px;
    display: flex;
    align-items: center;
    overflow: hidden;
    background-color: $primary-peach;
    color: $primary-white;
    border-radius: 15px;
    padding-left: 76px;

    img {
      position: absolute;
    }

    > img {
      height: 100%;
      top: 0;
      right: 0;
    }

    .bg-img-container img {
      top: -30px;
      right: -60px;
    }

    .text-container {
      width: 540px;
    }

    h1 {
      font-size: $heading-1-size;
      line-height: $heading-1-height;
      margin-bottom: 45px;
    }

    p {
      width: 445px;
      margin-bottom: 45px;
    }

    @media only screen and (max-width: $tablet-max-width-landscape) {
      height: 843px;
      text-align: center;
      align-items: flex-start;
      justify-content: center;
      padding-top: 65px;
      padding-left: 0;

      > img {
        height: 640px;
        top: 100px;
        left: 170px;
      }

      .bg-img-container {
        img {
          margin-left: auto;
          margin-right: auto;
          left: 0;
          right: 0;
          top: 285px;
        }
      }

      .text-container {
        z-index: 1;

        h1 {
          margin-bottom: 40px;
        }

        p {
          width: 450px;
          margin: 0 auto 25px;
        }
      }
    }

    @media only screen and (max-width: $phone-max-width) {
      width: 100%;
      border-radius: 0;
      padding-top: 78px;
      height: 843px;

      > img {
        left: 0;
      }

      .bg-img-container {
        top: 302px;
        height: 843px;
        background: url('~static/assets/home/desktop/image-hero-phone.png') center top;
        width:100%;
        position:absolute;

        img {
          visibility: hidden;
        }
      }

      .text-container {
        padding: 0 25px;

        h1 {
          font-size: 32px;
          font-weight: 500;
          line-height: 36px;
          margin-bottom: 30px;
        }

        p {
          width: 100%;
          font-size: 15px;
          line-height: 25px;
          margin-bottom: 25px;
        }
      }
    }
  }
</style>
