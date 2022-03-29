<template>
    <div>
        <div class="my-container">
            <div class="comic-container">
                <ComicCard
                    v-for="(element, index) in comics" :key="index"
                />
            </div>
        </div>
    </div>
</template>

<script>
import ComicCard from "./ComicCard.vue"

export default {
    name: "CurrentSeries",
    data: function() {
        return {
            comics: [
                {
                    title: "",
                    img: ""
                },
            ]
        }
    },
    components: {
        ComicCard
    }
}
</script>

<style lang="scss" scoped>
    @import "../assets/scss/partials/_variables.scss";

    div{
        background-color: $darkBlack;
        height: 80vh;

        .comic-container{
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            width: 90%;
            margin: 0 auto;

            .comic-element{
                width: calc(20% - (.8rem));
                margin: .1rem;
                background-color: white;
                padding: 1rem;
                text-align: center;

                img{
                    width: 100%;
                }
            }
        }
    }
    
</style>