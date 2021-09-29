<template>
  <main>
      <div class="container">
        <div class="rowIcons">
          <div class="iconInRow">
            <img src="@/assets/images/buy-comics-digital-comics.png" alt="Digital Comics">
            <p>DIGITAL COMICS</p>
          </div>
          <div class="iconInRow">
            <img src="@/assets/images/buy-comics-merchandise.png" alt="DC Merchandise">
            <p>DC MERCHANDISE</p>
          </div>          
          <div class="iconInRow">
            <img src="@/assets/images/buy-comics-subscriptions.png" alt="Subscription">
            <p>SUBSCRIPTION</p>
          </div>          
          <div class="iconInRow">
            <img src="@/assets/images/buy-comics-shop-locator.png" alt="Comic shop locator">
            <p>COMIC SHOP LOCATOR</p>
          </div>          
          <div class="iconInRow">
            <img src="@/assets/images/buy-dc-power-visa.svg" alt="DC Power Visa">
            <p>DC POWER VISA</p>
          </div>
        </div>
      </div>
  </main>
</template>

<script>
export default {
  name: 'MainBottom'
}
</script>

<style lang="scss" scoped>
@import '../assets/style/variables';

main {
  background-color: $cyanBandColor;

  .container{

    .rowIcons{

      display: flex;
      justify-content: space-evenly;
      padding: 30px 0;


      .iconInRow {

        display: flex;
        align-items: center;
        color: #fff;
        
      &-:last-child img {
          width: 55px;

      }

        img {
          height: 55px;
          
        }


        p {
          margin: 0 10px;
        }
      }
    }
  }
}


</style>