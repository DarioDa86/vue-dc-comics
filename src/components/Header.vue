<template>
  <header>
      <div class="container">
        <div class="logoDC">
            <img src="@/assets/images/dc-logo.png" alt="Logo DC">
        </div>
        <nav>
            <ul>
                <li><a href="#">CHARACTERS</a> </li>
                <li><a class="active" href="#">COMICS</a></li>
                <li><a href="#">MOVIES</a></li>
                <li><a href="#">TV</a></li>
                <li><a href="#">GAMES</a></li>
                <li><a href="#">COLLECTIBLES</a></li>
                <li><a href="#">VIDEOS</a></li>
                <li><a href="#">FANS</a></li>
                <li><a href="#">NEWS</a></li>
                <li><a href="#">SHOP</a></li>
            </ul>
        </nav>
      </div>
  </header>
</template>

<script>
export default {
    name: 'Header'
}
</script>

<style lang="scss" scoped>
@import '../assets/style/variables';

    .container {
        display: flex;
        align-items: center;
        justify-content: space-between;


        nav {
            margin: 20px 0;

            ul {
            display: flex;
            justify-content: center;
            list-style: none;

                a {
                    text-decoration: none;
                    margin: 10px;
                    color: $textNavColor;
                    font-size: 18px;
                    font-weight: Bold;

                    &.active {
                        color: $cyanBandColor;
                        padding-bottom: 46px;
                        border-bottom: 5px solid $cyanBandColor;
                    }
                }
            }
        }

        .logoDC {
            img {
                height: 80px;
                margin: 20px 0;
            }
        }
    }
</style>