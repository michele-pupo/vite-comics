<script>
    import AppNav from './components/AppNav.vue';
    import AppContent from './components/AppContent.vue';
    import AppBlueBundles from './components/AppBlueBundles.vue';
    import AppMain from './components/AppMain.vue';
    import AppFooter from './components/AppFooter.vue';

    export default{

    components: {
        AppNav,
        AppContent,
        AppBlueBundles,
        AppMain,
        AppFooter
    },

}
</script>

<template>
    
    <AppNav></AppNav>
    <AppContent></AppContent>
    <AppBlueBundles></AppBlueBundles>
    <AppMain></AppMain>
    <AppFooter></AppFooter>

</template>

<style lang="scss">
  @use './styles/general.scss' as *;
</style>
