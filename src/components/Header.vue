<template>
    <div>
        <div class="my-container">
            <div class="header-logo">
                <img src="../assets/img/dc-logo.png" alt="DC logo">
            </div>
            <nav class="header-nav">   
                <ul>
                    <li v-for="(element, index) in navList" :key="index">
                        <a href="#">
                            {{ element.text }}
                        </a>
                    </li>
                </ul>
            </nav>
        </div>
    </div>
</template>

<script>
export default {
    name : "IndexHeader",
    data: function(){
        return {
            navList: [
                {
                    text: "Characters",
                    active: false
                },
                {
                    text: "Comics",
                    active: false
                },
                {
                    text: "Movies",
                    active: false
                },
                {
                    text: "TV",
                    active: false
                },
                {
                    text: "Games",
                    active: false
                },
                {
                    text: "Collectibles",
                    active: false
                },
                {
                    text: "Videos",
                    active: false
                },
                {
                    text: "Fans",
                    active: false
                },
                {
                    text: "News",
                    active: false
                },
                {
                    text: "Shop",
                    active: false
                },
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
    @import "../assets/scss/partials/_variables.scss";

    div{
        margin-top: 1rem;
        margin-bottom: 1rem;
        height: 15vh;
    }

    div.my-container{
        display: flex;
        justify-content: space-between;
        align-items: center;
        height: 100%;
        

        img{
            height: 100%;
            padding: 1rem;
        }

        ul{
            display: flex;
            align-items: center;

            li{
                list-style-type: none;
                padding: 1rem;
                line-height: 12vh;

                a{
                    font-size: .8rem;
                    text-decoration: none;
                    color: black;
                    text-transform: uppercase;
                    font-weight: bold;
                }

                &:active,
                &.active{
                    border-bottom: $dcBlue 4px solid;
                }
            }
        }
    }

    header-nav,
    ul{
        height: 100%;
    }
</style>