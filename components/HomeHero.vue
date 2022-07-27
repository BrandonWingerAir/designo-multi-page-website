<template>
  <section>
    <img id="circle-bg" src="/assets/home/desktop/bg-pattern-hero-home.svg"/>
    <img id="phone-bg" src="/assets/home/desktop/image-hero-phone.png"/>
    <div>
      <h1>Award-winning custom designs and digital branding solutions</h1>
      <p>
        With over 10 years in the industry, we are experienced in creating fully responsive websites, app design, and engaging brand experiences. Find out more about our services.
      </p>
      <button class="btn-light">Learn more</button>
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

    img {
      position: absolute;

      &:first-of-type {
        height: 100%;
        top: 0;
        right: 0;
      }

      &:last-of-type {
        top: -30px;
        right: -60px;
      }
    }

    div {
      width: 540px;
      margin-left: 76px;
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
  }
</style>
