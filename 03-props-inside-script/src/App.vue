<script setup>
    import MainNavigation from './components/MainNavigation.vue';
    import SiteContent from './components/SiteContent.vue';
    import SiteFooter from './components/SiteFooter.vue';
</script>

<template>
    <header>
        <MainNavigation title="My Vue App" />
    </header>
    <main>
        <SiteContent/>
    </main>
    <footer>
        <!-- sitefooter komponens használata -->
        <SiteFooter/>
    </footer>
</template>

<style scoped>
</style>
