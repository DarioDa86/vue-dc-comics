<template>
    <header>
        <div class="container">
            <div class="logoDC">
                <img src="../assets/images/dc-logo.png" alt="Logo DC">
            </div>
            <nav>
                <ul>
                    <li v-for="(link, index) in menu" :key="index">
                        <a :href="link.url" >{{link.text}}</a> 
                    </li>
                </ul>
            </nav>
        </div>
        <Hero/>
    </header>
</template>

<script>
import Hero from '../components/Hero.vue';
export default {
    name: "Header",
    components: {
        Hero
    },
    data() {
        return {
            menu: [
                {
                    text: "CHARACTERS",
                    url:"#",
                    current: "false",
                },
                {
                    text: "COMICS",
                    url:"#",
                    current: "true",
                },
                {
                    text: "MOVIES",
                    url:"#",
                    current: "false",
                },
                {
                    text: "TV",
                    url:"#",
                    current: "false",
                },
                {
                    text: "GAMES",
                    url:"#",
                    current: "false",
                },
                {
                    text: "COLLECTIBLES",
                    url:"#",
                    current: "false",
                },
                {
                    text: "VIDEO",
                    url:"#",
                    current: "false",
                },
                {
                    text: "FANS",
                    url:"#",
                    current: "false",
                },
                {
                    text: "NEWS",
                    url:"#",
                    current: "false",
                },
                {
                    text: "SHOP",
                    url:"#",
                    current: "false",
                },
            ]
        }
    }
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

                    &:hover {
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