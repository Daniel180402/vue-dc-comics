<template>
    <main>

        <MainContent />
        <MainNav />
    </main>
</template>

<script>
import MainContent from './MainContent.vue';
import MainNav from './MainNav.vue';

export default {
    name : "IndexMain",
    components: {
        MainContent,
        MainNav
    }
}
</script>

<style lang="scss" scoped>

</style>