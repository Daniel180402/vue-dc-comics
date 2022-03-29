<template>
    <nav id="main-nav">
        <div class="my-container">
            <ul>
                <li v-for="(element, index) in listItem" :key="index">
                    <a href="#">
                        <img :src="element.img" alt="">
                        <h3>{{ element.name }}</h3>
                    </a>
                </li>
            </ul>
        </div>
    </nav>
</template>

<script>
export default {
    name: "MainNav",
    data: function() {
        return{
            listItem: [
                {
                    name: "Digital Comics",
                    img: require("../assets/img/buy-comics-digital-comics.png")
                },
                {
                    name: "DC Merchandise",
                    img: require("../assets/img/buy-comics-merchandise.png")
                },
                {
                    name: "Subscription",
                    img: require("../assets/img/buy-comics-shop-locator.png")
                },
                {
                    name: "Comic Shop Locator",
                    img: require("../assets/img/buy-comics-subscriptions.png")
                },
                {
                    name: "DC Power Visa",
                    img: require("../assets/img/buy-dc-power-visa.svg")
                }
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
    @import "../assets/scss/partials/_variables.scss";

    nav#main-nav{
        background-color: $dcBlue;
        height: 15vh;

        div.my-container{
            display: flex;
            justify-content: center;
            height: 100%;

            ul{
            display: flex;

            li{
                list-style-type: none;
                padding: 0 .6rem;
                line-height: 5.5vh;

                a{
                    font-size: .8rem;
                    text-decoration: none;
                    color: white;
                    text-transform: uppercase;
                    display: flex;
                    height: 100%;
                    align-items: center;

                    img{
                        height: 50%;
                        margin: 0 .8rem;
                    }
                }
            }
        }
        }
    }
</style>