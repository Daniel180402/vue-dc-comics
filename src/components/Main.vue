<template>
    <div>

        <ContentMain/>
        <CurrentSeries/>
        <MainNav/>

    </div>
</template>

<script>
import ContentMain from './ContentMain.vue'
import CurrentSeries from './CurrentSeries.vue'
import MainNav from './MainNav.vue'

export default {
    name : "IndexMain",
    components: {
        ContentMain,
        CurrentSeries,
        MainNav
    }
}
</script>

<style lang="scss" scoped>
    @import "../assets/scss/partials/_variables.scss";

    
</style>