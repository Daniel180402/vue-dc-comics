<template>
    <div id="main-content">
        <div class="jumbo">

        </div>
        <!-- <div class="my-container">
            <h2>Content</h2>
        </div> -->
    </div>
</template>

<script>
export default {
    name: "MainContent"
}
</script>

<style lang="scss" scoped>

    div#main-content{
        height: 60vh;

        .jumbo{
            height: 100%;
            background-image: url(../assets/img/jumbotron.jpg);
            
        }
    }
    // @import "../assets/scss/partials/_variables.scss";

    // div#main-content{
    //     background-color: $darkBlack;
    //     height: 15vh;
    //     line-height: 15vh;

    //     h2{
    //         color: white;
    //     }
    // }
</style>