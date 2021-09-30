<template>
  <footer>
    <div class="container">
      <div class="topFooter">

      </div>

      <div class="bottomFooter">

        <div class="signUp-Btn">
          <button>SIGN-UP NOW!</button>
        </div>

        <div class="socialIcons">
          <div class="textIcons">FOLLOW US</div>
          <img src="@/assets/images/footer-facebook.png" alt="Facebook">
          <img src="@/assets/images/footer-twitter.png" alt="Twitter">
          <img src="@/assets/images/footer-youtube.png" alt="Youtube">
          <img src="@/assets/images/footer-pinterest.png" alt="Pinterest">
          <img src="@/assets/images/footer-periscope.png" alt="Periscope">

        </div>


      </div>

    </div>
  </footer>
</template>

<script>
export default {
    name: 'Footer'
}
</script>

<style lang="scss" scoped>
@import '../assets/style/variables';

footer {
  background-color: $footerBottomBackColor;

  .bottomFooter {
    display: flex;
    justify-content: space-between;
    align-items: center;
    vertical-align: center;
    padding: 20px 0;

    .socialIcons {
      display: flex;
    }
  }
}

</style>