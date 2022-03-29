<template>
    <div>

        <ContentMain/>
        <MainNav/>

    </div>
</template>

<script>
import ContentMain from './ContentMain.vue'
import MainNav from './MainNav.vue'

export default {
    name : "IndexMain",
    components: {
        ContentMain,
        MainNav
    }
}
</script>

<style lang="scss" scoped>
    @import "../assets/scss/partials/_variables.scss";

    
</style>