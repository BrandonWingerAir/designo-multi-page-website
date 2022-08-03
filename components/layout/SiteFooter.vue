<template>
    <footer>
      <div class="content-margin">
        <SiteNavbarLight/>
        <hr>
        <div class="social-container">
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
            <a href="#!"><img src="~/static/assets/shared/desktop/icon-facebook.svg"></a>
            <a href="#!"><img src="~/static/assets/shared/desktop/icon-youtube.svg"></a>
            <a href="#!"><img src="~/static/assets/shared/desktop/icon-twitter.svg"></a>
            <a href="#!"><img src="~/static/assets/shared/desktop/icon-pinterest.svg"></a>
            <a href="#!"><img src="~/static/assets/shared/desktop/icon-instagram.svg"></a>
          </div>
        </div>
      </div>
    </footer>
</template>

<style lang="scss" scoped>
footer {
  background: $primary-black;
  width: 100%;
  height: 393px;
  overflow:hidden;

  hr {
    margin-bottom: 36px;
    border: none;
    height: 1px;
    background-color: #424242;
  }

  .social-container {
    display: grid;
    grid: 100% / 1fr 1fr 1fr;
    margin-bottom: 72px;
    color: #979797;

    h4 {
      font-size: $body-text-size;
      font-weight: 600;
      line-height: $body-text-height;
    }

    .contact-info a {
      color: #979797;
      font-weight: 600;
      display: block;
    }

    > :last-child {
      display: flex;
      justify-content: flex-end;
      align-items: center;

      a {
        margin-left: 16px;

        &:hover {
          filter: brightness(125%);
        }
      }
    }
  }

  @media only screen and (max-width: $tablet-max-width-landscape) {
    height: 423px;
  }

  @media only screen and (max-width: $phone-max-width) {
    height: 100%;

    hr {
      display: none;
    }

    .social-container {
      display: block;
      text-align: center;
      line-height: 26px;
      margin-bottom: 50px;

      div {
        margin-bottom: 35px;
      }

      .contact-info a {
        font-weight: 500;
      }

      > :last-child {
        justify-content: center;

        a {
          margin: 0 8px;
        }
      }
    }
  }
}
</style>
