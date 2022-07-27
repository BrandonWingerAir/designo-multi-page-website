<template>
  <footer>
    <div class="content-margin">
      <SiteContact/>
      <SiteNavbarLight/>
      <hr>
      <div id="social-container">
        <div>
          <h4>Designo Central Office</h4>
          <p>3886 Wellington Street</p>
          <p>Toronto, Ontario M9C 3J5</p>
        </div>
        <div class="contact-info">
            <h4>Contact Us (Central Office)</h4>
            <a href="tel:+">P : +1 253-863-8967</a>
            <a href="mailto:">M : contact@designo.co</a>
        </div>
        <div>
          <a href="#!">SOCIAL ICONS</a>
        </div>
      </div>
    </div>
  </footer>
</template>

<style lang="scss" scoped>
footer {
  background: $primary-black;
  color: $primary-white;
  width: 100%;
  height: 393px;

  > div:first-child {
    position: relative;
    top: -220px;
  }

  a {
    color: $primary-white;
  }

  hr {
    margin-bottom: 36px;
    border: none;
    height: 1px;
    background-color: #424242;
  }

  #social-container {
    display: grid;
    grid: 100% / 1fr 1fr 1fr;

    h4, p, a {
      color: #979797;
    }

    h4 {
      font-size: $body-text-size;
      font-weight: 600;
      line-height: $body-text-height;
    }

    .contact-info a {
      font-weight: 600;
      display: block;
    }
  }
}
</style>
