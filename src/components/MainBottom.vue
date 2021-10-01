<template>
  <main>
    <div class="container">
      <ul class="rowIcons">
        <li class="iconInRow" v-for="(icon, index) in icons" :key="index">
          <a href=""><img :src="icon.image" /></a>
          <a href="">{{ icon.text }}</a>
        </li>
      </ul>
    </div>
  </main>
</template>

<script>
export default {
  name: "MainBottom",
  data() {
    return {
      icons: [
        {
          image: require("../assets/images/buy-comics-digital-comics.png"),
          text: "DIGITAL COMICS",
          url: "#",
        },
        {
          image: require("../assets/images/buy-comics-merchandise.png"),
          text: "DC MERCHANDISE",
          url: "#",
        },
        {
          image: require("../assets/images/buy-comics-subscriptions.png"),
          text: "SUBSCRIPTION",
          url: "#",
        },
        {
          image: require("../assets/images/buy-comics-shop-locator.png"),
          text: "COMIC SHOP LOCATOR",
          url: "#",
        },
        {
          image: require("../assets/images/buy-dc-power-visa.svg"),
          text: "DC POWER VISA",
          url: "#",
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
@import "../assets/style/variables";

main {
  background-color: $cyanBandColor;

  .container {
    .rowIcons {
      display: flex;
      justify-content: space-evenly;
      padding: 30px 0;

      .iconInRow {
        display: flex;
        align-items: center;

        &:last-child img {
          height: 40px;
        }

        img {
          height: 55px;
        }

        a {
          margin: 0 10px;
          font-size: 18px;
          color: #fff;
          text-decoration: none;
        }
      }
    }
  }
}
</style>