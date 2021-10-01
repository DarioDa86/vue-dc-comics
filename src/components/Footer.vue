<template>
  <footer>
    <div class="container">
      <div class="topFooter">
        <div class="footerLeft">
          <div class="col-1">
            <h3>DC COMICS</h3>
            <ul>
              <li><a href="#">Charracters</a></li>
              <li><a href="#">Comics</a></li>
              <li><a href="#">Movies</a></li>
              <li><a href="#">TV</a></li>
              <li><a href="#">Games</a></li>
              <li><a href="#">Videos</a></li>
              <li><a href="#">News</a></li>
            </ul>
            <h3>SHOP</h3>
            <ul>
              <li><a href="#">Shop DC</a></li>
              <li><a href="#">Shop DC Collectibles</a></li>
            </ul>
          </div>
          <div class="col-2">
            <h3>DC</h3>
            <ul>
              <li><a href="#">Therms Of Use</a></li>
              <li><a href="#">Privacy policy(New</a></li>
              <li><a href="#">Ad Choices</a></li>
              <li><a href="#">Advertising</a></li>
              <li><a href="#">Jobs</a></li>
              <li><a href="#">Subscription</a></li>
              <li><a href="#">Talent Workshops</a></li>
              <li><a href="#">CPSC Certificates</a></li>
              <li><a href="#">Ratings</a></li>
              <li><a href="#">Shop Help</a></li>
              <li><a href="#">Contact Us</a></li>
            </ul>
          </div>
          <div class="col-3">
            <h3>SITES</h3>
            <ul>
              <li><a href="#">DC</a></li>
              <li><a href="#">MAD Magazine</a></li>
              <li><a href="#">DC Kids</a></li>
              <li><a href="#">DC Universe</a></li>
              <li><a href="#">DC Power Visa</a></li>
            </ul>
          </div>
        </div>

        <div class="footerRight"></div>
      </div>
    </div>
    <div class="bgFooter">
      <div class="bottomFooter container">
        <div class="signUp-Btn">
          <a href="#"><button>SIGN-UP NOW!</button></a>
        </div>

        <div class="socialIcons">
          <div class="textIcons">FOLLOW US</div>
          <a href="#"
            ><img src="../assets/images/footer-facebook.png" alt="Facebook"
          /></a>
          <a href="#"
            ><img src="../assets/images/footer-twitter.png" alt="Twitter"
          /></a>
          <a href="#"
            ><img src="../assets/images/footer-youtube.png" alt="Youtube"
          /></a>
          <a href="#"
            ><img src="../assets/images/footer-pinterest.png" alt="Pinterest"
          /></a>
          <a href="#"
            ><img src="../assets/images/footer-periscope.png" alt="Periscope"
          /></a>
        </div>
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  name: "Footer",
};
</script>

<style lang="scss" scoped>
@import "../assets/style/variables";

footer {
  background-image: url(../assets/images/footer-bg.jpg);
  background-repeat: no-repeat;
  background-size: cover;

  .topFooter {
    display: flex;

    .footerLeft {
      display: flex;
      color: #fff;
      width: 30%;
      margin: 30px 0;

      .col-1 {
        width: calc(100% / 3);
      }

      .col-2 {
        width: calc(100% / 3);
      }

      .col-3 {
        width: calc(100% / 3);
      }
    }

    .footerRight {
      width: 70%;
      background-image: url(../assets/images/dc-logo-bg.png);
      background-repeat: no-repeat;
      background-position: right center;
    }
  }

  .bgFooter {
    background-color: $footerBottomBackColor;

    .bottomFooter {
      display: flex;
      justify-content: space-between;
      align-items: center;
      padding: 20px 0;

      .signUp-Btn {
        button {
          padding: 15px 10px;
          border-radius: 0;
          border: 3px solid $cyanBandColor;
          background-color: transparent;
          color: #fff;
          font-size: 16px;
        }
      }

      .socialIcons {
        display: flex;
        align-items: center;
        justify-content: space-between;
        color: $cyanBandColor;

        img {
          margin: 0 10px;
        }

        .textIcons {
          font-size: 18px;
          font-weight: bold;
          margin-right: 15px;
        }
      }
    }
  }
}
</style>